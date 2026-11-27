# LexProof Forensic Engine — Arquitectura Pericial Digital

> Motor de análisis forense digital y preservación de evidencia conforme a estándares internacionales **ISO/IEC 27037** (cadena de custodia) e **ISO/IEC 27042** (análisis e interpretación pericial).

[![GitHub Repo](https://img.shields.io/badge/GitHub-cmansilla%2Flexproof--forensic--engine-181717?logo=github)](https://github.com/cmansilla/lexproof-forensic-engine)
[![Standard: ISO 27037](https://img.shields.io/badge/Standard-ISO%2FIEC%2027037%2F27042-blue.svg)]()
[![Legal: FRE 902(14)](https://img.shields.io/badge/Admissibility-FRE%20Rule%20902(14)-green.svg)]()
[![Python: 3.11+](https://img.shields.io/badge/Python-3.11+-yellow.svg)]()

---

## 📌 Especificación Técnica del Sistema

- **Cadena de Custodia Inmutable:**
  - Hashing criptográfico dual (SHA-256 + BLAKE3) generado en el momento exacto de la ingesta.
  - Generación de sellos de tiempo deterministas y logs forenses auditables para admisibilidad legal bajo regla **FRE 902(14)**.
- **Detección Anti-Anti-Forensics (CAF v3.0):**
  - Detección de *EXIF Spoofing*, manipulación de metadatos y re-compresiones mediante software de edición.
  - Análisis de artefactos de cuantización JPEG y matrices DCT para identificar inserciones de contenido generado por IA.
- **Reportes Periciales:** Exportación automatizada de dictámenes periciales estructurados con árbol de dependencias probatorias (*Why-Trail*).

---

## 🏗️ Topología del Sistema

```mermaid
flowchart TD
    A["Evidencia Digital (Archivos / Imágenes / PDFs)"] --> B["Ingesta & Hash Dual (SHA-256 / BLAKE3)"]
    B --> C["Módulo de Preservación ISO 27037"]
    C --> D["Motor de Análisis CAF v3.0 (Anti-Spoofing)"]
    D --> E["Auditor de Matrices DCT & Metadatos"]
    E --> F["Why-Trail: Árbol de Razonamiento Pericial"]
    F --> G["Dictamen Forense Certificado (FRE 902(14))"]
```

```text
┌────────────────────────────────────────────────────────┐
│             Evidencia Digital (Archivos/PDF)           │
└───────────────────────────┬────────────────────────────┘
                            │
                            ▼
┌────────────────────────────────────────────────────────┐
│        Ingesta & Hash Dual (SHA-256 / BLAKE3)          │
└───────────────────────────┬────────────────────────────┘
                            │
                            ▼
┌────────────────────────────────────────────────────────┐
│     Análisis CAF v3.0 (Detección Manipulación IA)      │
└───────────────────────────┬────────────────────────────┘
                            │
                            ▼
┌────────────────────────────────────────────────────────┐
│     Dictamen Pericial Certificado (ISO 27042 / FRE)    │
└────────────────────────────────────────────────────────┘
```
