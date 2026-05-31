# TFG – Clasificación semántica de documentación aeroespacial

Repositorio de notebooks y datasets del Trabajo de Fin de Grado 
"Aplicación de modelos de Deep Learning para la clasificación semántica 
de documentación aeroespacial" (UC3M, 2026).

## Contenido

### Notebooks

| Notebook | Descripción |
|----------|-------------|
| `01_transform_taxonomy.ipynb` | Transformación y preprocesamiento de la taxonomía PAE |
| `02_semantic_analysis_taxonomy.ipynb` | Análisis semántico de las categorías de la taxonomía |
| `03_filter_projects_engineering.ipynb` | Filtrado del dataset original por dominio de ingeniería |
| `04_filter_projects_aero.ipynb` | Filtrado léxico por palabras clave aeroespaciales |
| `05_analysis_corpus_pae.ipynb` | Análisis exploratorio del corpus de 5.374 proyectos |
| `05_1_analysis_cleaned_corpus_pae.ipynb` | Análisis exploratorio del corpus final de 733 proyectos |
| `06_semantic_analysis_corpus_pae.ipynb` | Depuración semántica y construcción del corpus final |
| `07_classification_corpus_pae.ipynb` | Clasificación baseline de proyectos contra la taxonomía PAE |

### Datasets

| Fichero | Descripción |
|---------|-------------|
| `EUproject.xlsx` | Dataset original (79.840 proyectos). **Descargar desde [Google Drive](https://docs.google.com/spreadsheets/d/14Pk52TO5O5nuFc5kzieSNH5qEpjspM3i/edit?usp=sharing)** |
| `aerotaxLimpio_v3.xlsx` | Taxonomía PAE original en Excel |
| `aerotax_transformado.csv` | Taxonomía PAE procesada (151 categorías) |
| `EUproject_aerospatial_filtered_5000.csv` | 5.374 proyectos tras primera iteración de keywords |
| `EUproject_aerospatial_filtered_10000.csv` | 12.047 proyectos tras segunda iteración de keywords |
| `pae_aero_corpus.csv` | Corpus final de 733 proyectos aeroespaciales |

> **Nota:** Los ficheros `EUproject_engineering_filtered.csv` y 
> `EUproject_engineering_clean.csv` no están incluidos por su tamaño (>100MB). 
> Se generan ejecutando el notebook `03_filter_projects_engineering.ipynb`.

## Orden de ejecución

1. Descargar `EUproject.xlsx` desde el enlace de Google Drive
2. Ejecutar los notebooks en orden numérico (01 → 07)

## Requisitos

- Python 3.x
- pandas, numpy, scikit-learn
- sentence-transformers
- matplotlib
