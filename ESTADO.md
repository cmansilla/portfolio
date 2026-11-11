# ESTADO DEL PROYECTO: PORTFOLIO & SHOWCASE TECNICO

**Fecha de Guardado:** 10 de Noviembre de 2026 — 19:35:00 -05:00  
**Ubicación en Disco:** `/home/usuario/Pycode/portfolio-landing`  
**Autor:** `mmansillaf`  
**Host de Desarrollo:** Lenovo ThinkPad T14 Gen 1 (Ubuntu 24.04 LTS)  

---

## 1. Resumen de Entregables Generados

1. **Landing Page en Producción (`index.html`)**:
   * **Ruta:** `/home/usuario/Pycode/portfolio-landing/index.html`
   * **Stack:** HTML5, Tailwind CSS (CDN), Tipografía Google (`Plus Jakarta Sans` + `JetBrains Mono`).
   * **Estética:** Dark Mode de alto impacto (estilo Linear/Vercel) con `#07090e`, mallas de luz ambiental, bordes de cristal (`backdrop-blur-xl`).
   * **Componente Interactivo:** Micro-simulador de búsqueda Tantivy v0.26 embebido (JavaScript nativo, filtrado sub-milisegundo &lt;0.4ms sobre resoluciones del Tribunal Fiscal).
   * **Gobernanza de Copywriting:** Sustituido el término absoluto "cero alucinación" por *"Sistemas con Verificación Determinista y Trazabilidad Documental Auditada"*.

2. **Auditoría de Proveedores de Hosting & Cloud (Resultados Clave)**:
   * **Descartados para Producción:**
     * Render Free: Destruye bases de datos PostgreSQL a los 30 días de creadas.
     * Vercel Hobby: Prohíbe formalmente cualquier uso comercial o profesional bajo ToS.
   * **Seleccionados por Arquitectura:**
     * **Frontend / Portafolio:** Cloudflare Pages ($0/mes, CDN global, DDoS ilimitado, ToS comercial permitido).
     * **Bases de Datos Serverless:** Neon Postgres (scale-to-zero tras 5 min, 100 CU-horas/mes) y Turso (libSQL Edge).
     * **Almacenamiento sin Egreso:** Cloudflare R2 / Tigris Data ($0 tarifas de transferencia).
     * **Demos Pesadas:** VPS Contabo existente (`167.86.108.85`) expuesto de forma segura vía Cloudflare Tunnel (sin abrir puertos en firewall).

---

## 2. Inventario de Proyectos Integrados en el Showcase

* **Saleman Resoluciones** (Tier 1 / WSM 93.05): Motor Tantivy en Rust, respuestas en submilisegundos sobre 5,000 documentos.
* **InmobiliariaData** (Tier 1 / WSM 93.20): Pipeline sobre 25,292 avisos inmobiliarios con DuckDB y Polars.
* **LexProof Forensic Engine** (Tier 2 / WSM 89.28): Motor forense digital ISO 27037/27042 y detección anti-spoofing.
* **SUNAT Expert AI Fork v2** (Tier 1 / WSM 94.10): LLM tributario entrenado con 53.7k diálogos SFT sobre grafo DuckDB.
* **LocalSearchEngine V2** (Tier 2 / WSM 88.82): Motor semántico offline con LanceDB y frontend en Svelte.
* **Hermes Skills Ecosistema** (Tier 2 / WSM 85.22): Catálogo de 118 skills estructuradas para agentes autónomos.

---

## 3. Próximos Pasos al Reiniciar

```bash
# 1. Abrir y revisar la landing en el navegador
google-chrome /home/usuario/Pycode/portfolio-landing/index.html

# 2. Despliegue directo a Cloudflare Pages (opción CLI)
npx wrangler pages deploy /home/usuario/Pycode/portfolio-landing --project-name=portfolio-mansilla

# 3. Vincular con GitHub mmansillaf
cd /home/usuario/Pycode/portfolio-landing
# git remote add origin https://github.com/mmansillaf/portfolio.git
# git push -u origin main
```
