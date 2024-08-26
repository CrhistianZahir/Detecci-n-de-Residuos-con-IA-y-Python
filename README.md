# Estimación de la contaminación por residuos en el Canal Bogotá de la ciudad de Cúcuta empleando visión artificial

## Acerca del Proyecto
Este proyecto se presento como tesis de pregrado para graduarme como ingeniero electrónico de la Universidad Francisco de Paula Santander, en el que obtuve el reconocimiento de tesis laureada al obtener la máxima nota 5.0/5.0.
En este proyecto desarrolle un modelo computacional con la capacidad de detectar la presencia de residuos a través de imágenes, y generar un archivo csv con el número de residuos detectados y el porcentaje de ocupación de estos residuos. Emplee tecnologías como visión artificial, inteligencia artificial, Machine Learning, Deep Learning, procesamiento de imágenes, el lenguaje de programación Python, Jupyter Notebook, Anaconda, y Google Colab. Desarrolle un modelo clasificador de imágenes (residuos) utilizando un algoritmo Haar Cascade.
Construí un conjunto de datos para el entrenamiento de modelos de detección de objetos, realizando los procesos de recopilación de datos, etiquetado de datos y preparación del conjunto de datos. Entrene arquitecturas de detección Deep Learning (Faster R-CNN, SSD MobileNet V2 y SSD MobileNet V2 FPNLite) utilizando Tensorflow. Implemente los modelos de visión artificial entrenados en una Raspberry Pi. Se desarrolló un algoritmo de programación para estimar el nivel de contaminación por medio del calculo del area ocupada por los residuos utilizando procesamiento de imágenes en Python. Implementé visualizaciones de datos para observar el rendimiento y los resultados del modelo computacional.

## Habilidades técnicas y herramientas
- Investigación, Redacción
- Inteligencia Artificial, Machine Learning, Deep Learning y Visión por Computador
- Python
- Visual Studio Code, Jupyter Notebook y Google Colab
- Scikit-Learn, Tensorflow, Keras, NumPy, Pandas, OpenCV, Matplotlib, Seaborn

## Autor
Crhistian Zahir Diaz Garcia

## Pregunta Problema
¿Cómo utilizar la visión artificial para identificar residuos y estimar el nivel de contaminación del Canal Bogotá de la ciudad de Cúcuta?

## Objetivos

**Objetivo General**
Estimar automáticamente la contaminación por residuos en el Canal Bogotá de la ciudad de Cúcuta mediante visión artificial.

**Objetivos Específicos**
- Caracterizar las zonas para la adquisición de imágenes a fin de realizar la identificación automática de los residuos.
- Generar un conjunto de datos con imágenes propias referentes a los tipos de residuos presentes en el Canal Bogotá de la ciudad de Cúcuta.
- Realizar un algoritmo basado en herramientas de visión artificial para estimar la contaminación e identificar residuos en el Canal Bogotá de la ciudad de Cúcuta.
- Evaluar la implementación de la visión artificial para estimar la contaminación por residuos.

## Conclusiones
- La caracterización detallada de las zonas permitió seleccionar los sitios del Canal Bogotá que representan una muestra significativa de los residuos que se generan en el área urbana en los sectores comerciales, empresariales y residenciales de la ciudad de Cúcuta. Esta caracterización facilitó la construcción del conjunto de datos propio, determinando en este proceso los residuos que se presentan en este tipo de entorno, los residuos que se visualizaron con mayor frecuencia fueron, las bolsas plásticas, vasos plásticos, botellas plásticas, cartón, botellas de vidrio, platos de icopor, porta comidas de icopor y residuos textiles.
- La generación del conjunto de datos propio permitió obtener imágenes que representan las características del Canal Bogotá, el conjunto de imágenes estaba formado por características como lo es la presencia de agua, residuos, habitantes de calle, árboles, plantas, vegetación, aves y escombros de construcción. Con el acceso a esta información se facilitó el entrenamiento de las arquitecturas de detección de objetos y se obtuvo un modelo con la capacidad de detectar residuos en condiciones reales que se presentan en las zonas del Canal Bogotá.
- La investigación permitió validar las técnicas de segmentación por color y umbralización como unas herramientas efectivas del área del procesamiento de imágenes para identificar la presencia de residuos en imágenes en entornos no controlados por medio de la separación de los objetos de interés del fondo, en el que se obtuvo una exactitud del 80.7% al identificar correctamente 92 residuos de 100 posibles.
- En la ejecución y evaluación del sistema de visión artificial en el conjunto de datos de prueba se determinó que, el modelo de detección de residuos que mejor se adapta a sistemas embebidos con características de hardware limitadas es la arquitectura SSD MobileNet V2, mientras que, el modelo con mejor desempeño en cuanto a parámetros de precisión, Recall y puntaje F1 es la arquitectura Faster R-CNN, sin embargo, esta arquitectura es mucho más robusta en comparación con la SSD MobileNet V2, por lo tanto, no es la más indicada para implementarse en un sistema embebido debido a que esta requiere de unas características de hardware más exigentes.
- La implementación del modelo computacional en la Raspberry Pi 3B+ con 1GB de memoria RAM permitió identificar que se alcanzó un alto uso de recursos como lo es la CPU y la memoria RAM, resultando en un tiempo de inferencia de 6 minutos, mientras que, la ejecución del modelo desde el ordenador tiene un tiempo de inferencia de 1 segundo, por lo tanto, se concluye que para fines de implementación y mantener la calidad de funcionamiento del sistema, se recomienda implementarse en dispositivos con al menos 4GB de memoria RAM.
