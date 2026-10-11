# Dataset
Origen: [AI-Lab-Makerere/beans](https://huggingface.co/datasets/AI-Lab-Makerere/beans), imágenes de hojas de frijol etiquetadas por enfermedad, hoja manchada y hoja sana.

Campos de origen: `image` (imagen RGB o convertible a RGB), `labels` (entero categórico). Las etiquetas se leen dinámicamente de `features["labels"].names`: `angular_leaf_spot`, `bean_rust`, `healthy`.

Partición usada: `test`. Selección reproducible: `shuffle(seed=42)` y primeras 60 imágenes (configurable). `src/descargar_dataset.py` genera `data/manifiesto_test.csv` con índice, ID y nombre de etiqueta.
