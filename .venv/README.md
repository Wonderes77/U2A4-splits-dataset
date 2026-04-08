# U2A4 — Splits reproducibles de un dataset abierto

**Autora:** Esmeralda Gómez Huerta  
Práctica de la Unidad 2 — Ciberfísica e Inteligencia Artificial Aplicada    
Partición train/test reproducible aplicada al dataset **Wine Quality** de UCI.

---

## Descripción

Este repositorio contiene el notebook y los archivos generados de la práctica U2A4,
donde se aplica una partición train/test con semilla fija sobre un dataset abierto,
con el objetivo de generar splits reproducibles para el entrenamiento y evaluación
de modelos de inteligencia artificial.

---

## Estructura del repositorio

```
U2A4-splits-dataset/
├── U2A4_notebook.ipynb       # Notebook principal con todo el código y la nota técnica
├── winequality-red.csv       # Dataset original descargado de UCI
├── winequality.names         # Descripción oficial del dataset
└── splits/
    ├── train.csv             # Conjunto de entrenamiento (80% — 1,279 filas)
    └── test.csv              # Conjunto de prueba (20% — 320 filas)
```

---

## Dataset

| Campo | Detalle |
|---|---|
| **Nombre** | Wine Quality (vino tinto) |
| **Fuente** | UCI Machine Learning Repository |
| **URL** | https://archive.ics.uci.edu/dataset/186/wine+quality |
| **Total de registros** | 1,599 filas |
| **Variables** | 11 características químicas + 1 variable objetivo (quality) |

---

## Parámetros de la partición

| Parámetro | Valor |
|---|---|
| Proporción | 80% train / 20% test |
| Semilla (random_state) | 42 |
| Criterio | Estratificado por `quality` (stratify=y) |

---

## Cómo ejecutar

1. Clona el repositorio:
   ```bash
   git clone https://github.com/Wonderes77/U2A4-splits-dataset.git
   ```
2. Coloca el archivo `winequality-red.csv` en la misma carpeta que el notebook.
3. Abre `U2A4_notebook.ipynb` en Jupyter Notebook.
4. Ejecuta todas las celdas de arriba a abajo.

---

## Créditos del dataset

> P. Cortez, A. Cerdeira, F. Almeida, T. Matos and J. Reis.  
> *Modeling wine preferences by data mining from physicochemical properties.*  
> In Decision Support Systems, Elsevier, 47(4):547-553, 2009.

Dataset disponible en: https://archive.ics.uci.edu/dataset/186/wine+quality
