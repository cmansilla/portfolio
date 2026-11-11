# ESTADO DEL PROYECTO: PORTFOLIO & SHOWCASE TECNICO

**Fecha de Guardado:** 11 de Noviembre de 2026 — 14:02:00 -05:00  
**Ubicación en Disco:** `/home/usuario/Pycode/portfolio-landing`  
**Autor:** Christian Mansilla (`cmansilla`)  
**Host de Desarrollo:** Lenovo ThinkPad T14 Gen 1 (Ubuntu 24.04.5 LTS)  
**Repositorio Remoto:** [https://github.com/cmansilla/portfolio](https://github.com/cmansilla/portfolio)  
**Rama / Commit:** `main` (`f425672` o posterior) — **100% Sincronizado con origin/main**  
**Despliegue Live:** [https://cmansilla.github.io/portfolio/](https://cmansilla.github.io/portfolio/)

---

## 1. Resumen de Entregables y Cambios Consolidados

1. **Reorientación Profesional a GenAI & LLMOps**:
   - Actualizado el rol a **GenAI & LLMOps Engineer** en `README.md` e `index.html`.
   - Énfasis en **inferencia distribuida de baja latencia (Gemini SSE, Groq), arquitecturas RAG híbridas (Rust Tantivy sub-1ms, LanceDB, SQLite WAL) y post-entrenamiento supervisado (SFT 53k)**.

2. **Remediación Total de Enlaces 404 & Especificaciones Técnicas**:
   - Se crearon 7 documentos completos de arquitectura técnica en el directorio `projects/` dentro del repositorio público:
     - `projects/audit-cpe-app.md`: Motor Go nativo (`SingleFlight`, mutex, caché atómica SUNAT, Excel).
     - `projects/saleman-resoluciones.md`: Búsqueda jurisprudencial en Rust (Tantivy P99 < 0.42ms, FastAPI, Gemini SSE).
     - `projects/inmobiliaria-data.md`: Pipeline OLAP columnar (DuckDB, Polars, 25k registros geoespaciales).
     - `projects/sunat-expert-ai.md`: Pipeline SFT (53.7k pares ChatML, DuckDB Grafo, QLoRA 4-bit).
     - `projects/local-search-engine.md`: Buscador semántico offline LanceDB (14k fragmentos) y Svelte.
     - `projects/lexproof-forensic-engine.md`: Motor pericial ISO 27037/27042 y detección de IA (FRE 902).
     - `projects/hermes-skills.md`: Orquestación de 118 skills, protocolo MCP y aislamiento en Git worktrees.
   - Reemplazada la sección de comandos locales triviales (`python3 -m http.server`) por la **Matriz de Proyectos de Ingeniería y Repositorios Centrales**.
   - Enlaces en `index.html` actualizados a las rutas públicas de GitHub.
   - **Prueba Empírica:** 100% de los enlaces verificados con respuesta `HTTP 200 OK`.

3. **Arquitectura y Visualización**:
   - Todos los documentos y diagramas Mermaid cumplen con la directiva estricta de orientación descendente (`flowchart TD`) y **doble renderizado universal con cajas Unicode/ASCII**.

---

## 2. Inventario de Proyectos Integrados

| Proyecto | Especialidad | Stack Tecnológico | Especificación & Arquitectura |
| :--- | :--- | :--- | :--- |
| **Audit CPE Engine** | Auditoría tributaria y concurrencia | Go (Pure), SingleFlight, Mutex | [`projects/audit-cpe-app.md`](projects/audit-cpe-app.md) |
| **Saleman Resoluciones** | Búsqueda jurisprudencial P99 < 0.42ms | Rust (Tantivy), FastAPI, SQLite WAL | [`projects/saleman-resoluciones.md`](projects/saleman-resoluciones.md) |
| **InmobiliariaData** | Pipeline analítico geoespacial | DuckDB, Polars, PyArrow | [`projects/inmobiliaria-data.md`](projects/inmobiliaria-data.md) |
| **SUNAT Expert AI** | Modelo de dominio y SFT | ChatML (53.7k diálogos), DuckDB Grafo | [`projects/sunat-expert-ai.md`](projects/sunat-expert-ai.md) |
| **LocalSearchEngine V2** | Búsqueda vectorial offline | LanceDB, Apache Arrow, Svelte | [`projects/local-search-engine.md`](projects/local-search-engine.md) |
| **LexProof Forensic** | Cadena de custodia digital | ISO 27037/27042, CAF v3.0, FRE 902 | [`projects/lexproof-forensic-engine.md`](projects/lexproof-forensic-engine.md) |
| **Hermes Skills** | Orquestación multi-agente | MCP Protocol, Git Worktrees | [`projects/hermes-skills.md`](projects/hermes-skills.md) |

---

## 3. Comandos para Reanudar la Sesión

```bash
# 1. Acceder al repositorio del portafolio
cd /home/usuario/Pycode/portfolio-landing

# 2. Verificar sincronización con GitHub
git status

# 3. Abrir la versión en producción
google-chrome https://cmansilla.github.io/portfolio/
```
