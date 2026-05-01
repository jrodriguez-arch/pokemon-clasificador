# Mi Proyecto: Clasificador de Pokemon por Tipo

## Descripcion
Este proyecto consiste en una aplicación web que clasifica imágenes de Pokémon según su tipo principal: fuego, agua o planta. El modelo fue entrenado usando Transfer Learning con ResNet50 y luego desplegado en Streamlit Cloud para que cualquier persona pueda probarlo subiendo una imagen.

## Demo
https://pokemon-clasificador-l33k8bwyqpome9ey87qcwc.streamlit.app/

## Por que este tema
Elegí Pokémon porque es un tema conocido, visualmente atractivo y fácil de entender para cualquier persona. Además, los tipos fuego, agua y planta tienen diferencias visuales interesantes, aunque algunos Pokémon pueden confundirse por sus colores, fondos o diseños.


## Dataset
- Total de imagenes: 245
- Clases: - fuego: 53 imágenes
  - agua: 114 imágenes
  - planta: 78 imágenes
- Fuentes: de donde vinieron las imagenes

## Resultados
Mejor accuracy obtenido: 66%

| Clase | Precision | Recall | F1 |
|-------|-----------|--------|-----|
| fuego | 0.47 | 0.90 | 0.62 |
| agua | 0.80 | 0.55 | 0.65 |
| planta | 0.77 | 0.67 | 0.71 |

## Analisis de errores
El modelo tuvo más dificultad clasificando algunos Pokémon de agua, ya que varias imágenes fueron confundidas con fuego. Esto puede deberse a que algunas imágenes tienen fondos coloridos, poses diferentes o elementos visuales que no representan claramente el tipo del Pokémon.  
También se observó overfitting, porque el accuracy de entrenamiento fue mayor que el accuracy de validación.

## Aprendizajes
Lo más difícil fue lograr que el modelo entrenado funcionara correctamente en Streamlit Cloud, especialmente por problemas de compatibilidad entre versiones de TensorFlow/Keras. Aprendí la importancia de usar la misma lógica de preprocesamiento en entrenamiento y en la app, además de revisar logs para encontrar errores reales. También reforcé el uso de Transfer Learning para construir un clasificador funcional sin entrenar una CNN desde cero.

## Tecnologias usadas
- Python, TensorFlow/Keras
- Transfer Learning con ResNet50
- Streamlit para interfaz
- Streamlit Cloud para deploy
- GitHub

## Autor
Jonathan Rodriguez