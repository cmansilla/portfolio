# ESTADO DEL PROYECTO: PORTFOLIO & SHOWCASE TECNICO

**Fecha de Guardado:** 26 de Noviembre de 2026 — 18:12:00 -05:00  
**Ubicación en Disco:** `/home/usuario/Pycode/portfolio-landing`  
**Autor:** Christian Mansilla (`cmansilla`)  
**Host de Desarrollo:** Lenovo ThinkPad T14 Gen 1 (Ubuntu 24.04.5 LTS)  
**Repositorio Remoto:** [https://github.com/cmansilla/portfolio](https://github.com/cmansilla/portfolio)  
**Rama / Commit:** `main` (`97818f6` o posterior) — **100% Sincronizado con origin/main**  
**Despliegue Live:** [https://cmansilla.github.io/portfolio/](https://cmansilla.github.io/portfolio/)  
**Showcase Especializado RAG:** [https://cmansilla.github.io/portfolio/rag-showcase.html](https://cmansilla.github.io/portfolio/rag-showcase.html)

---

## 1. Resumen de Entregables y Cambios Consolidados (Sesión 26-Nov-2026)

1. **Incorporación del Showcase Especializado RAG & Retrieval**:
   - Creada la SPA [`rag-showcase.html`](rag-showcase.html) con arquitectura modular, diseño dark mode, paleta Tailwind (Emerald/Cyan/Purple) y visualizadores interactivos de código con fragmentos nucleares y métricas operativas.
   - Vinculación directa desde el header y la barra de filtros del portafolio principal (`index.html`).

2. **Integración de 3 Nuevas Fichas Técnicas de Arquitectura RAG**:
   - `projects/graphrag-juridico-hibrido.md`:
     - Extracción determinista en Python/C ($0.00 USD en tokens, <4 min de ingesta).
     - Graph Traversal en SQLite WAL con Common Table Expressions (CTE) recursivas con latencia <15 ms.
     - Invariantes de vigencia y trazabilidad de derogaciones tácitas.
   - `projects/sunarp-rag-grounder.md`:
     - Recuperación híbrida paralela (`pgvector` HNSW cosine + BM25 `tsvector`).
     - Fusión determinista Reciprocal Rank Fusion (RRF $k=60$) y Cross-Encoder Reranker.
     - Validador neurosimbólico Ley 31814 (anclaje N1-N6 y circuit breaker de confianza 0.75).
   - `projects/casaciones-search-engine-500k.md`:
     - Pipeline masivo para 500,000 sentencias de la Corte Suprema en PDF.
     - Gating OCR condicional (<80 chars/página activa PaddleOCR 300 DPI, ahorrando >70% de cómputo GPU).
     - Pseudonimización BPE-safe conforme a la Ley 29733 y Parent-Child Chunking (512 tokens vector / considerando íntegro LLM).

3. **Ampliación del Catálogo en `index.html` y `README.md`**:
   - Catálogo ampliado de 6 a 9 proyectos en producción.
   - Botón de filtrado directo "RAG & Grafos (3)".
   - 100% de enlaces verificados y validados sin referencias rotas.

---

## 2. Inventario Consolidado de Proyectos en el Portafolio (13 Proyectos)

| # | Proyecto | Especialidad | Stack Tecnológico | Especificación & Arquitectura |
|---|:---|:---|:---|:---|
| 1 | **GraphRAG Jurídico Híbrido** | RAG sobre grafos & SQLite CTE | SQLite WAL, CTEs <15ms, Parsers C/Regex | [`projects/graphrag-juridico-hibrido.md`](projects/graphrag-juridico-hibrido.md) |
| 2 | **Algoritmo Jurídico v4** | Motor tri-políglota P99 < 0.42ms | Rust (Tantivy), Go (MCP), Python | [`projects/algoritmo-juridico-v4.md`](projects/algoritmo-juridico-v4.md) · [Repo](https://github.com/cmansilla/algoritmojuridico-v4) |
| 3 | **Tribunal Fiscal Harvester** | Ingesta masiva 216k RTFs (MEF) | curl_cffi JA3, SQLite WAL, Cloud Offload | [`projects/tribunal-fiscal-harvester.md`](projects/tribunal-fiscal-harvester.md) · [Repo](https://github.com/cmansilla/tribunal-fiscal-harvester) |
| 4 | **CEJ Judicial Scraper** | Cosecha automatizada Poder Judicial | Playwright CDP, Radware Bypass, SHA-256 | [`projects/cej-judicial-scraper.md`](projects/cej-judicial-scraper.md) · [Repo](https://github.com/cmansilla/cej-judicial-scraper) |
| 5 | **SUNARP Chat AI & Grounder** | RAG híbrido y canal ciudadano | pgvector HNSW, BM25, RRF (k=60), Meta API | [`projects/sunarp-rag-grounder.md`](projects/sunarp-rag-grounder.md) |
| 6 | **Casaciones Search Engine 500k** | Búsqueda procesal masiva | 500k PDFs, Gating OCR 300DPI, Parent-Child | [`projects/casaciones-search-engine-500k.md`](projects/casaciones-search-engine-500k.md) |
| 7 | **Audit CPE Engine** | Auditoría tributaria y concurrencia | Go (Pure), SingleFlight, Mutex | [`projects/audit-cpe-app.md`](projects/audit-cpe-app.md) |
| 8 | **Saleman Resoluciones** | Búsqueda jurisprudencial P99 < 0.42ms | Rust (Tantivy), FastAPI, SQLite WAL | [`projects/saleman-resoluciones.md`](projects/saleman-resoluciones.md) |
| 9 | **InmobiliariaData** | Pipeline analítico geoespacial | DuckDB, Polars, PyArrow | [`projects/inmobiliaria-data.md`](projects/inmobiliaria-data.md) |
| 10 | **SUNAT Expert AI** | Modelo de dominio y SFT | ChatML (53.7k diálogos), DuckDB Grafo | [`projects/sunat-expert-ai.md`](projects/sunat-expert-ai.md) |
| 11 | **LocalSearchEngine V2** | Búsqueda vectorial offline | LanceDB, Apache Arrow, Svelte | [`projects/local-search-engine.md`](projects/local-search-engine.md) |
| 12 | **LexProof Forensic** | Cadena de custodia digital | ISO 27037/27042, CAF v3.0, FRE 902 | [`projects/lexproof-forensic-engine.md`](projects/lexproof-forensic-engine.md) |
| 13 | **Hermes Skills** | Orquestación multi-agente | MCP Protocol, Git Worktrees | [`projects/hermes-skills.md`](projects/hermes-skills.md) · 118+ Skills |

---

## 3. Instrucciones de Verificación Post-Reinicio

```bash
# 1. Acceder al repositorio del portafolio
cd /home/usuario/Pycode/portfolio-landing

# 2. Verificar estado limpio de Git
git status

# 3. Comprobar páginas desplegadas en Cloudflare / GitHub Pages
curl -I https://cmansilla.github.io/portfolio/
curl -I https://cmansilla.github.io/portfolio/rag-showcase.html
```
