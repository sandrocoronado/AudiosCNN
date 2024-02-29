# Separación de fuentes musicales utilizando redes convolucionales

En este proyecto, empleamos la inteligencia computacional, específicamente las redes convolucionales (CNN), para separar las fuentes de distintas obras musicales.

## Descripción del método

Las redes neuronales convolucionales nos permiten analizar las señales de audio por secciones más pequeñas, lo que nos ayuda a obtener características específicas de las mismas. Estas características se utilizan luego para separar las fuentes musicales.

Para aplicar este método, es necesario realizar algunos tratamientos previos a la señal de audio. Primero, convertimos la señal estéreo en su representación en tiempo y frecuencia mediante la Transformada de Tiempo Corto de Fourier (STFT). La entrada de la red convolucional será la matriz correspondiente a la magnitud de esta representación tiempo-frecuencia. Además, se guarda la fase de la señal, ya que será necesaria para la reconstrucción de las señales tras la separación de fuentes utilizando la Transformada de Tiempo Corto de Fourier Inversa (ISTFT).

## Aplicación en audio

Las redes neuronales convolucionales son especialmente útiles para el procesamiento de imágenes (matrices según dimensiones en píxeles). En nuestro caso, aplicamos esta arquitectura a matrices bidimensionales que representan las características tiempo-frecuencia del audio obtenidas mediante la STFT.

Este enfoque nos permite trabajar con representaciones complejas del audio y extraer características relevantes para la separación de fuentes musicales.
