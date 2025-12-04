# 🛡️ Compliance Check: Auditoría Normativa y Gobernanza con IA

### 📌 Misión del Módulo
Este directorio aloja soluciones de **Ingeniería de Prompts** diseñadas para la "Primera Línea de Defensa" en departamentos de Cumplimiento.
El objetivo es utilizar LLMs (Large Language Models / Modelos Grandes de Lenguaje) para realizar escaneos preventivos de documentos corporativos, asegurando su alineación con marcos regulatorios estrictos antes de que lleguen a la mesa del Compliance Officer (Oficial de Cumplimiento).

### 📖 Glosario de Estándares Soportados
Estos prompts han sido calibrados basándose en los textos legales oficiales de:
* **RGPD (Reglamento General de Protección de Datos):** Normativa europea 2016/679 sobre privacidad y datos personales.
* **ISO 27001 (International Organization for Standardization 27001):** Estándar internacional para la gestión de la seguridad de la información.
* **LSC (Ley de Sociedades de Capital):** Normativa española que regula el funcionamiento de las sociedades mercantiles.
* **AML (Anti-Money Laundering / Prevención de Blanqueo de Capitales):** Protocolos para evitar el lavado de dinero.

### ⚙️ Metodología: "Zero Trust & Evidence Based"
A diferencia de los prompts creativos, en Compliance aplicamos una filosofía de **Confianza Cero**:
1.  **Temperature 0:** Eliminamos cualquier aleatoriedad.
2.  **Cita Obligatoria:** La IA no puede marcar algo como "Incorrecto" sin citar el artículo de la ley o el párrafo de la norma ISO (International Organization for Standardization) que se está violando.
3.  **Salida Binaria:** El resultado debe tender a `CUMPLE` / `NO CUMPLE` para facilitar la auditoría automática.

### 📂 Proyectos Detallados
| Archivo | Caso de Uso | Normativa Aplicada |
| :--- | :--- | :--- |
| `auditor-web-rgpr.md` | Verificador automático de textos legales en páginas web (Políticas de Privacidad y Cookies). | RGPD (Art. 13 y 14) |

---
