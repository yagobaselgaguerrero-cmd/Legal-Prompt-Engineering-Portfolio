# 🤖 Automatización Procesal: Ingeniería de Datos Legales

### 📌 Descripción del Módulo
Este directorio contiene instrucciones para convertir texto jurídico no estructurado (sentencias, demandas, BOE) en **datos estructurados (JSON, CSV)** procesables por software.
El objetivo es eliminar la entrada manual de datos en los despachos y alimentar bases de datos de jurisprudencia automáticamente.

### ⚙️ Metodología Técnica
* **Modelo:** GPT-4o (Modo JSON activado).
* **Técnica:** *Data Extraction* + *Zero-Shot*.
* **Formato de Salida:** JSON estricto (listo para API o integración con Excel).

### 📂 Proyectos en esta carpeta
| Archivo | Descripción | Stack |
| :--- | :--- | :--- |
| `extractor-sentencias-json.md` | Extracción automática de metadatos (Juez, Cuantía, Fallo) de sentencias civiles para alimentar un Excel/CRM. | JSON Output |

---
