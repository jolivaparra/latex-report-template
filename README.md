# UdeC Project Template

**Plantilla Modular para Informes de Proyectos.**
*Departamento de Ingeniería Eléctrica - Universidad de Concepción*

Este repositorio es una plantilla ("Scaffolding") diseñada para documentos académicos de gran extensión. Implementa una arquitectura modular que separa estrictamente el contenido, la lógica de compilación y los recursos, utilizando estándares de nombres en inglés (`snake_case`) para máxima compatibilidad y orden.

---

## 📂 Estructura del Proyecto (Project Structure)

El proyecto sigue una jerarquía clara para mantener la cordura a medida que el documento crece.

```text
/
├── main.tex                  # Archivo Maestro (Orquestador). NO escribir contenido aquí.
├── references.bib            # Base de datos bibliográfica (BibTeX/BibLaTeX).
├── udec-core.sty             # Backend: Matemáticas, física y configuración base.
├── udec-report.sty           # Frontend: Estilos visuales, portadas y formatos.
│
├── content/                  # SOLO TEXTO (.tex)
│   ├── abstract.tex          # Resumen Ejecutivo / Abstract.
│   ├── sections/             # Capítulos numerados del informe.
│   │   ├── 01_introduction.tex
│   │   ├── 02_theoretical_background.tex
│   │   └── ...
│   └── appendices/           # Anexos y apéndices (Datasheets, demostraciones).
│
├── figures/                  # RECURSOS GRÁFICOS (Imágenes .png, .jpg, .pdf)
│   ├── 01_intro/             # Subcarpetas coincidentes con las secciones.
│   ├── 02_theory/
│   └── logos/
│
├── tables/                   # TABLAS COMPLEJAS (.tex, .csv)
│   └── specs_summary.tex     # Código LaTeX de tablas grandes para importar.
│
└── code/                     # CÓDIGO FUENTE
    └── data_processing/      # Scripts de Python/MATLAB/C usados en la tesis.