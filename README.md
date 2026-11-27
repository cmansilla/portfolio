# Christian Mansilla — Technical Portfolio & Architecture Showcase

[![GitHub Pages](https://img.shields.io/badge/Demo_En_Vivo-cmansilla.github.io%2Fportfolio-emerald?style=for-the-badge&logo=github)](https://cmansilla.github.io/portfolio/)
[![RAG Showcase](https://img.shields.io/badge/RAG_Showcase-Sistemas_de_Recuperacion-059669?style=for-the-badge&logo=diagramsdotnet&logoColor=white)](https://cmansilla.github.io/portfolio/rag-showcase.html)
[![Tailwind CSS](https://img.shields.io/badge/Tailwind_CSS-38B2AC?style=for-the-badge&logo=tailwind-css&logoColor=white)](https://tailwindcss.com)
[![Rust Tantivy](https://img.shields.io/badge/Rust-Tantivy_FTS-DEA584?style=for-the-badge&logo=rust&logoColor=white)](https://github.com/quickwit-oss/tantivy)

> **Sitio en producción disponible en:**  
> 🌐 **[https://cmansilla.github.io/portfolio/](https://cmansilla.github.io/portfolio/)**  
> 🔍 **[Showcase Especializado de Arquitecturas RAG & Retrieval](https://cmansilla.github.io/portfolio/rag-showcase.html)**

---

## 📌 ¿Qué contiene este repositorio?

Este repositorio aloja el código fuente del **Portafolio de Ingeniería y Demostración Técnica de Christian Mansilla (GenAI & LLMOps Engineer)**, enfocado en **inferencia distribuida de baja latencia (Google Gemini con streaming SSE nativo, Groq), arquitecturas de recuperación híbrida (GraphRAG, Tantivy Rust sub-1ms, LanceDB, SQLite WAL, pgvector) y post-entrenamiento supervisado (SFT) de modelos de lenguaje** para entornos de producción de misión crítica.

### Componentes Clave:

1. **Simulador Interactivo de Búsqueda Tantivy (Rust)**:
   - Micro-simulador en vivo en el cliente que emula el índice invertido de *Tantivy v0.26* sobre 5,000 resoluciones del Tribunal Fiscal peruano.
   - Demuestra filtrado léxico instantáneo con métricas de latencia dinámica (**P99 < 0.42 ms**).

2. **RAG & Retrieval Architecture Showcase (`rag-showcase.html`)**:
   - Presentación interactiva y profunda de 3 motores RAG avanzados: **GraphRAG Jurídico Híbrido** (SQLite CTEs <15ms), **SUNARP Chat AI** (HNSW + BM25 + RRF k=60) y **Casaciones Search Engine 500k** (Gating OCR + Parent-Child).

3. **Catálogo de Proyectos Auditados**:
   - **GraphRAG Jurídico Híbrido**: Ontología legal con traversals recursivos deterministas y cero costo en ingesta.
   - **SUNARP Chat AI & RAG Grounder**: Orientación registral ciudadana con anclaje normativo N1-N6 y handoff humano.
   - **Casaciones Search Engine 500k**: Pipeline a gran escala sobre 500,000 sentencias con pseudonimización BPE-safe.
   - **Saleman Resoluciones**: Motor de búsqueda en Rust con persistencia SQLite WAL.
   - **LocalSearchEngine V2**: Buscador semántico offline con LanceDB y PyArrow (14,256 chunks vectorizados).
   - **InmobiliariaData**: Pipeline de analítica geoespacial con DuckDB y Polars sobre 25,292 avisos en Lima.
   - **SUNAT Expert AI**: Modelo de dominio tributario con 53.7k pares conversacionales en formato ChatML.

4. **Métricas de Infraestructura y Topología**:
   - Documentación visual de la arquitectura híbrida: despliegue en CDN estático, túneles SSH/Zero-Trust y granjas de servidores en Linux.

---

## 🚀 Proyectos de Ingeniería y Repositorios Centrales

| Proyecto | Especialidad | Stack Tecnológico | Especificación & Arquitectura |
| :--- | :--- | :--- | :--- |
| **GraphRAG Jurídico Híbrido** | RAG sobre grafos & SQLite CTE | SQLite WAL, CTEs <15ms, Parsers C/Regex | [Ver Arquitectura GraphRAG](projects/graphrag-juridico-hibrido.md) · [Ver Showcase](https://cmansilla.github.io/portfolio/rag-showcase.html#graphrag) |
| **Algoritmo Jurídico v4** | Motor tri-políglota P99 < 0.42ms | Rust (Tantivy), Go (MCP), Python | [Ver Ficha Técnica](projects/algoritmo-juridico-v4.md) · [GitHub Repo](https://github.com/cmansilla/algoritmojuridico-v4) |
| **SUNARP Chat AI & Grounder** | RAG híbrido y canal ciudadano | pgvector HNSW, BM25, RRF (k=60), Meta API | [Ver Arquitectura SUNARP RAG](projects/sunarp-rag-grounder.md) · [Ver Showcase](https://cmansilla.github.io/portfolio/rag-showcase.html#sunarp) |
| **Casaciones Search Engine 500k** | Búsqueda procesal a gran escala | 500k PDFs, Gating OCR 300DPI, Parent-Child | [Ver Arquitectura 500k](projects/casaciones-search-engine-500k.md) · [Ver Showcase](https://cmansilla.github.io/portfolio/rag-showcase.html#casaciones) |
| **Tribunal Fiscal Harvester** | Ingesta masiva 216k RTFs (MEF) | curl_cffi JA3, SQLite WAL, Cloud Offload | [Ver Ficha Técnica](projects/tribunal-fiscal-harvester.md) · *(Repo Privado)* |
| **CEJ Judicial Scraper** | Cosecha automatizada Poder Judicial | Playwright CDP, Radware Bypass, SHA-256 | [Ver Ficha Técnica](projects/cej-judicial-scraper.md) · *(Repo Privado)* |
| **Audit CPE Engine** | Auditoría tributaria y concurrencia | Go (Pure), SingleFlight, Mutex | [Ver Arquitectura Go (`v2.1.0`)](projects/audit-cpe-app.md) |
| **Saleman Resoluciones** | Búsqueda jurisprudencial P99 < 0.42ms | Rust (Tantivy), FastAPI, SQLite WAL | [Ver Arquitectura Rust/FastAPI](projects/saleman-resoluciones.md) |
| **InmobiliariaData** | Pipeline analítico geoespacial | DuckDB, Polars, PyArrow | [Ver Arquitectura OLAP](projects/inmobiliaria-data.md) · 25k rows |
| **SUNAT Expert AI** | Modelo de dominio y SFT | ChatML (53.7k diálogos), DuckDB Grafo | [Ver Arquitectura SFT / Grafo](projects/sunat-expert-ai.md) |
| **LocalSearchEngine V2** | Búsqueda vectorial offline | LanceDB, Apache Arrow, Svelte | [Ver Arquitectura LanceDB](projects/local-search-engine.md) |
| **LexProof Forensic** | Cadena de custodia digital | ISO 27037/27042, CAF v3.0, FRE 902 | [Ver Arquitectura Forense](projects/lexproof-forensic-engine.md) |
| **Hermes Skills** | Orquestación multi-agente | MCP Protocol, Git Worktrees | [Ver Arquitectura Agéntica](projects/hermes-skills.md) · 118+ Skills |

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
