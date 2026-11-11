# Christian Mansilla — Technical Portfolio & Architecture Showcase

[![GitHub Pages](https://img.shields.io/badge/Demo_En_Vivo-cmansilla.github.io%2Fportfolio-emerald?style=for-the-badge&logo=github)](https://cmansilla.github.io/portfolio/)
[![Tailwind CSS](https://img.shields.io/badge/Tailwind_CSS-38B2AC?style=for-the-badge&logo=tailwind-css&logoColor=white)](https://tailwindcss.com)
[![Rust Tantivy](https://img.shields.io/badge/Rust-Tantivy_FTS-DEA584?style=for-the-badge&logo=rust&logoColor=white)](https://github.com/quickwit-oss/tantivy)

> **Sitio en producción disponible en:**  
> 🌐 **[https://cmansilla.github.io/portfolio/](https://cmansilla.github.io/portfolio/)**

---

## 📌 ¿Qué contiene este repositorio?

Este repositorio aloja el código fuente del **Portafolio de Ingeniería y Demostración Técnica de Christian Mansilla (GenAI & LLMOps Engineer)**, enfocado en **inferencia distribuida de baja latencia (Google Gemini con streaming SSE nativo, Groq), arquitecturas de recuperación híbrida (índices invertidos en Rust sub-1ms, LanceDB, SQLite WAL) y post-entrenamiento supervisado (SFT) de modelos de lenguaje** para entornos de producción de misión crítica.

### Componentes Clave:

1. **Simulador Interactivo de Búsqueda Tantivy (Rust)**:
   - Micro-simulador en vivo en el cliente que emula el índice invertido de *Tantivy v0.26* sobre 5,000 resoluciones del Tribunal Fiscal peruano.
   - Demuestra filtrado léxico instantáneo con métricas de latencia dinámica (**P99 < 0.42 ms**).

2. **Catálogo de Proyectos Auditados**:
   - **Saleman Resoluciones**: Motor de búsqueda en Rust con persistencia SQLite WAL.
   - **LocalSearchEngine V2**: Buscador semántico offline con LanceDB y PyArrow (14,256 chunks vectorizados).
   - **InmobiliariaData**: Pipeline de analítica geoespacial con DuckDB y Polars sobre 25,292 avisos en Lima.
   - **SUNAT Expert AI**: Modelo de dominio tributario con 53.7k pares conversacionales en formato ChatML.

3. **Métricas de Infraestructura y Topología**:
   - Documentación visual de la arquitectura híbrida: despliegue en CDN estático, túneles SSH/Zero-Trust y granjas de servidores en Linux.

---

## 🚀 Proyectos de Ingeniería y Repositorios Centrales

| Proyecto | Especialidad | Stack Tecnológico | Repositorio / Estado |
| :--- | :--- | :--- | :--- |
| **Audit CPE Engine** | Auditoría tributaria y concurrencia | Go (Pure), SingleFlight, Mutex | [`audit-cpe-app`](https://github.com/mmansillaf/audit-cpe-app) · `v2.1.0` |
| **Saleman Resoluciones** | Búsqueda jurisprudencial P99 < 0.42ms | Rust (Tantivy), FastAPI, SQLite WAL | [`saleman_resoluciones`](https://github.com/mmansillaf/saleman_resoluciones) |
| **InmobiliariaData** | Pipeline analítico geoespacial | DuckDB, Polars, PyArrow | [`inmobiliaria-data`](https://github.com/mmansillaf/inmobiliaria-data) · 25k rows |
| **SUNAT Expert AI** | Modelo de dominio y SFT | ChatML (53.7k diálogos), DuckDB Grafo | *Validación SFT / ThinkPad P53* |

---

## 🛠️ Stack Tecnológico

- **Frontend**: HTML5, Tailwind CSS (JIT vía CDN), JavaScript Vanilla.
- **Tipografía**: `Plus Jakarta Sans` (lectura ejecutiva) + `JetBrains Mono` (datos técnicos y código).
- **Despliegue**: GitHub Pages / Cloudflare Pages.
- **Licencia**: MIT.

---

## 📬 Contacto
- **GitHub**: [github.com/cmansilla](https://github.com/cmansilla)
- **LinkedIn**: [linkedin.com/in/christian-mansilla](https://linkedin.com/in/christian-mansilla)
- **Email**: christian.mansilla@outlook.es
