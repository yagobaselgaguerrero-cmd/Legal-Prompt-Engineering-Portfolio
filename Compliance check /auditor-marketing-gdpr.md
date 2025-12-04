# Proyecto: Auditoría Automática de Campañas (GDPR & LSSI)

## 1. El Problema
Los departamentos de Marketing generan contenido mucho más rápido de lo que el departamento Legal puede revisar. Esto provoca cuellos de botella o, peor aún, que se envíen correos electrónicos (newsletters) que violan el RGPD o la Ley de Competencia Desleal por descuido.

## 2. La Solución (The Prompt)
Un "Sistema de Semáforo" basado en IA. El prompt analiza el *copy* publicitario y detecta riesgos legales basándose en la normativa española (LSSI, RGPD, Consumo), ofreciendo correcciones antes de la publicación.

### 🛠️ Configuración
* **Rol:** Senior Compliance Officer (España).
* **Técnica:** *Chain of Thought* (Razonamiento paso a paso) + *Risk Scoring*.
* **Objetivo:** Detectar "Dark Patterns" y violaciones de privacidad.

### 💻 El Código del Prompt (Input)

```text
/* SYSTEM ROLE */
Eres un experto en Compliance Digital y Privacidad (GDPR/LSSI) en España.
Tu tarea es auditar textos de marketing antes de que sean enviados.

/* INSTRUCTIONS */
Analiza el siguiente borrador de correo electrónico.
1. Identifica frases que puedan suponer un riesgo legal.
2. Cita la normativa infringida (aprox).
3. Clasifica el riesgo (ALTO/MEDIO/BAJO).
4. Propón una redacción alternativa ("Wording Sugerido") que mantenga el impacto comercial pero cumpla la ley.

Formato de salida: Tabla Markdown.

/* INPUT TEXT (DRAFT) */
"¡Hola! Hemos visto que entraste en la web de nuestra competencia, así que te añadimos a nuestra lista VIP.
Si compras nuestro suplemento vitamínico, curarás tu ansiedad en 24 horas garantizado.
Haz clic aquí o te cobraremos 10€ por inactividad."
