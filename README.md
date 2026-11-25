# FORM-IC-01 — Investigación individual: Arquitecturas distribuidas en la industria

Investigación técnica sobre la implementación de **Arquitectura Orientada a Eventos (EDA)** en **Atlassian** mediante su plataforma de eventos en tiempo real **StreamHub** y **Apache Kafka (AWS MSK)**, desarrollada como actividad preparatoria para el Informe Académico Individual `TA-IND-02`.

## Estructura del repositorio

```text
.
├── main.tex           # Archivo principal en LaTeX (carátula, análisis de 1 página, evidencias y referencias)
├── referencias.bib    # Bibliografía en formato BibLaTeX (estilo IEEE con DOIs verificados)
├── main.pdf           # Documento PDF compilado (se incorpora en la versión final)
├── capturas/          # Evidencia gráfica de lectura y anotación sobre la fuente oficial
└── README.md          # Instrucciones de compilación y dependencias
```

## Requisitos y dependencias

* **Distribución LaTeX:** MiKTeX o TeX Live (2023 o superior).
* **Compilador:** `pdflatex`
* **Motor bibliográfico:** `biber`
* **Archivo principal:** `main.tex`
* **Paquetes requeridos:**
  * Idioma y codificación: `inputenc` (`utf8`), `fontenc` (`T1`), `babel` (`spanish`), `csquotes`
  * Maquetación y tipografía: `geometry`, `lmodern`, `microtype`, `titlesec`, `enumitem`
  * Gráficos y enlaces: `graphicx`, `float`, `caption`, `xcolor`, `xurl`, `hyperref`
  * Citas y referencias IEEE: `biblatex` (`backend=biber`, `style=ieee`, paquete `biblatex-ieee`)

## Orden de compilación

Desde la raíz del repositorio, ejecutar la secuencia completa (`pdflatex` → `biber` → `pdflatex` → `pdflatex`):

```bash
pdflatex main.tex
biber main
pdflatex main.tex
pdflatex main.tex
```
