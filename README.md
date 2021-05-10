# Desafío 4: Predicción de atributos de una canción

En este desafío deberán imitar el algoritmo de recomendación de spotify.

En el repositorio se adjunta un Dataset (en formato .csv) con distintos atributos de muchas canciones. Estas canciones ya han sido procesadas, por lo que se tendrán atributos relacionados a qué tan bailables son, el tempo, que tan ruidosa es, entre otros. Su objetivo será generar un modelo de red neuronal que pueda predecir si una canción le gusta a una persona o no.

- Leer el Dataset.
- Implementar (sin uso de librerías que lo hagan) y entrenar un perceptrón multicapa para la tarea de clasificación. Para esto se debe dividir los datos en entrenamiento y pruebas (70/30 sugerido).
- Con los datos de prueba, calcule la precisión (accuracy) de la predicción.


## Datos Adicionales: Información sobre cada columna del Dataset

Estos datos (Excepto la label y la columna 0) fueron extraídos la API de spotify, la cuál pueden revisar mediante [el siguiente link](https://developer.spotify.com/documentation/web-api/reference/#object-tuneabletrackobject).

    - Columna 0: Float. id de la canción. Este dato no es relevante para la predicción.
    
    - Acoustiness:  [0-1] medida de qué tan acústica es la canción.
    
    - danceability:  Float [0-1] medida de qué tan bailable es la canción.
    
    - duration_ms: Entero. duración en ms de la canción.
    
    - energy:  Float [0-1] medida conceptual de la intensidad y actividad de una canción.
    
    - instrumentalness:  Float [0-1] medida de qué tan seguro está el algoritmo de que no hay partes vocales en la canción.
    
    - key:  Entero [0-11] el tono de la canción; ejemplo: 0 = C, 1 = C♯/D♭, 2 = D, etc.
    
    - liveness:  Float [0-1] medida de qué tan seguro está el algoritmo de que hay público en vivo.
    
    - loudness:  Float. el promedio en ruidez de una canción, el rango tiende a ser entre -60 y 0 db
    
    - mode:   Entero modalidad (mayor o menor)(1 o 0 respectivamente) de la canción.
    
    - popularity:  Float [0-100] medición de la popularidad de una canción. Se calcula mediante el número total de reproducciones de una canción y qué tan recientes son estas.
    
    - speechiness:  Float [0-1] medida de qué tan presente son las palabras habladas dentro de la canción. ejemplo: un podcast será más cercano a 1.0
    
    - tempo:  Float. el tempo estimado de la canción, en bpm.
    
    - time_signature: Entero [1-5] medida del compás de la canción.
    
    - valence:  Float [0-1] medida que está relacionada con la positividad de una canción. Valores más cercanos a 1.0 serán de canciones que suenan más positivamente (feliz, eufórico, etc).
    
    - label:  Binario [0-1] si al usuario le gustó la canción o no.
    