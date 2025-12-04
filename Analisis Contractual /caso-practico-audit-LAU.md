# Proyecto: Auditoría Automática de Contratos de Alquiler (LAU)

## 1. El Problema (The Pain Point)
Los inquilinos y propietarios a menudo firman contratos descargados de internet que contienen cláusulas nulas de pleno derecho según la **Ley de Arrendamientos Urbanos (LAU)** española. Revisar esto manualmente lleva tiempo y requiere conocimiento experto actualizado.

## 2. La Solución (The Prompt)
He diseñado un flujo de instrucciones (prompt chain) que actúa como un **Auditor Legal Estricto**.

### 🛠️ Configuración del Prompt
* **Rol (System):** Abogado experto en Derecho Inmobiliario en España (Senior Associate).
* **Restricción (Constraint):** Solo puedes basarte en la LAU vigente. Si algo es "injusto" pero "legal", márcalo como VÁLIDO. Solo marca como NULO lo que viole la ley explícitamente.
* **Formato de Salida:** Tabla Markdown.

### 💻 El Código del Prompt (Input)

```text
# SYSTEM ROLE
Actúa como un abogado experto en la Ley de Arrendamientos Urbanos (LAU) de España.
Tu tarea es auditar el texto que te proporcionaré delimitado por triple comilla.

# INSTRUCCIONES
1. Analiza cada cláusula una por una.
2. Compara el contenido con la normativa imperativa de la LAU (especialmente Art. 6 sobre nulidad de pactos).
3. Genera un informe de auditoría.

# FORMATO DE RESPUESTA REQUERIDO (JSON)
Devuelve el resultado en una tabla con estas columnas:
- "Texto Sospechoso"
- "Veredicto" (VÁLIDO / NULO)
- "Fundamento Jurídico" (Cita el artículo exacto)
- "Explicación Humana" (Breve explicación para el cliente)

# INPUT (Texto del contrato a analizar)
"""
CLÁUSULA TERCERA.- DURACIÓN. El contrato tendrá una duración de un año.
El inquilino renuncia expresamente al derecho de prórroga forzosa.
Si el inquilino se va antes de los 6 meses, deberá pagar una penalización de 5.000 euros.
El propietario podrá entrar en la vivienda una vez al mes para inspeccionarla.
"""

