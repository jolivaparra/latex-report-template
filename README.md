# UdeC Project Template

**Plantilla Modular para Informes de Proyectos.**
*Departamento de Ingeniería Eléctrica - Universidad de Concepción*

Este repositorio es una plantilla diseñada para documentos académicos de gran extensión. Implementa una arquitectura modular que separa estrictamente el contenido, la lógica de compilación y los recursos, utilizando estándares de nombres en inglés (`snake_case`) para máxima compatibilidad y orden.

---

## 📂 Estructura del Proyecto (Project Structure)

El proyecto sigue una jerarquía clara para mantener la cordura a medida que el documento crece.

```text
/
├── main.tex                  # Archivo Maestro (Orquestador). NO escribir contenido aquí.
├── references.bib            # Base de datos bibliográfica (BibTeX/BibLaTeX).
├── udec-report.sty             # Backend: Paquetes, configuración base, estilos, portadas y formatos.
│
├── content/                  # SOLO TEXTO (.tex)
│   ├── abstract.tex          # Resumen / Abstract.
│   ├── sections/             # Capítulos numerados del informe.
│   │   ├── 01_introduction.tex
│   │   ├── 02_theoretical_background.tex
│   │   └── ...
│   └── appendices/           # Anexos y apéndices (Datasheets, demostraciones, etc.).
│
├── figures/                  # RECURSOS GRÁFICOS (Imágenes .png, .jpg, .pdf)
│   ├── 01_intro/             # Subcarpetas coincidentes con las secciones.
│   ├── 02_theory/
│   └── logos/
│
├── tables/                   # TABLAS COMPLEJAS (.tex, .csv)
│   ├── 01_intro/             # Subcarpetas coincidentes con las secciones.
│   └── 02_theory/
│
└── code/                     # CÓDIGO FUENTE usado (Opcional)
    ├── c/     
    ├── matlab/
    └── python/
```