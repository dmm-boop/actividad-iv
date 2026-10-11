# Actividad IV - Gestión de Proyectos de Inteligencia Artificial

# Visión por computadora: enfermedades en hojas de frijol

Proyecto educativo y reproducible para comparar **tres modelos de CLIP zero-shot** en clasificación de imágenes de hojas de frijol: mancha angular, roya y hoja sana. No requiere entrenamiento.

## Estructura
- `notebooks/Actividad_IV_Gestión_de_Proyectos_de_Inteligencia_Artificial.ipynb`: Colab con GPU, dependencias, autenticación opcional, dataset, inferencia, métricas, latencia y conclusiones.
- `src/descargar_dataset.py`: genera manifiesto del dataset.
- `data/README.md`: Dataset utilizado, procedencia y campos.
- `results/Actividad IV Gestión de Proyectos de Inteligencia Artificial.docx`: Reporte técnico de la actividad.
- `requirements.txt`: Dependencias utilizadas.


## Ejecución
1. Abrir el notebook en [Google Colab](https://colab.research.google.com/).
2. `Entorno de ejecución > Cambiar tipo de entorno de ejecución > T4 GPU` (si está disponible).
3. Ejecutar todas las celdas en orden. La autenticación de HuggingFace es **opcional** para modelos públicos.


## Modelos utilizados
`openai/clip-vit-base-patch32`, `openai/clip-vit-base-patch16`, `openai/clip-vit-large-patch14`.

## Conclusiones
De acuerdo con los resultados obtenidos el modelo recomendado es clip-vit-base-patch32 ya que combina la mayor precisión observada con la menor latencia y una carga de parámetros mucho menor que por ejemplo el modelo clip-vit-large-patch14

