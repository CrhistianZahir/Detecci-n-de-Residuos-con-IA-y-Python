# Estimación de la contaminación por residuos en el Canal Bogotá de la ciudad de Cúcuta empleando visión artificial

## Acerca de
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

## Introducción
En el presente trabajo de investigación se desarrolló un modelo computacional con la capacidad de realizar la identificación de residuos por medio del uso de herramientas de visión artificial, así como la estimación de los niveles de contaminación por residuos por medio del procesamiento de imágenes. Partiendo inicialmente de la obtención de un conjunto de datos formado propio, se continua con el desarrollo de un algoritmo que permite determinar el nivel de contaminación por residuos en imágenes, seguidamente se lleva a cabo la configuración y entrenamiento de la arquitectura de detección de residuos. Asimismo, una vez entrenada la arquitectura se procede a cargarse e implementarse, finalizando con la evaluación del desempeño del modelo para estimar y detectar la contaminación por residuos en zonas del Canal Bogotá de la ciudad de Cúcuta.

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

## Referencias
Alcaldía de San José de Cúcuta. (2022). Remueven 4 toneladas de basuras del canal Bogotá. https://cucuta.gov.co/remueven-4-toneladas-de-basuras-del-canal-bogota/
Álvarez-Sanchez, T., Alvarez-Cedillo, J. A., & Cavillo-Téllez, A. (2021). Detección de basura utilizando aprendizaje máquina y aprendizaje intensivo. Número Especial de La Revista Aristas: Investigación Básica y Aplicada, 8(16), 167–173.
Aprende Machine Learning. (2020). Modelos de Detección de Objetos. https://www.aprendemachinelearning.com/modelos-de-deteccion-de-objetos/
ArcGIS Pro. (n.d.). Cómo funciona Calcular precisión para la detección de objetos. Retrieved November 3, 2023, from https://pro.arcgis.com/es/pro-app/latest/tool-reference/image-analyst/how-compute-accuracy-for-object-detection-works.htm
Bala Priya C. (2022). ¿Qué es Jupyter Notebook y cómo instalarlo? https://geekflare.com/es/jupyter-notebook-intro-and-installation/
Barba-Guamán, L. R. (2021). Uso de técnicas deep learning para reconocimiento de objetos en áreas rurales (Disertación Doctoral). Universidad Politécnica De Madrid. Madrid, España.
Benito-Úbeda, M. (2009). INTRODUCCIÓN A LOS SISTEMAS EMBEBIDOS (SSEE). In Apuntes de: Sistemas embebidos (2009) (pp. 1–30). Dpto. IIC Universidad de Murcia.
Caracol Radio. (2023). Habitantes piden solución al problema ambiental del canal Bogotá. https://caracol.com.co/2023/06/21/damnificados-por-ola-invernal-de-2020-volvieron-a-protestar-frente-a-la-alcaldia-de-cucuta/
Castillo-Suárez, J. (2020). Sistema seleccionador de botellas mediante visión artificial en Raspberry pi (Trabajo Final de Máster). Universidad Politécnica de Valencia.
Catalán-Urzúa, A. (2019). Técnicas de procesamiento digital de imágenes. REVISTA DE MARINA. https://revistamarina.cl/es/articulo/tecnicas-de-procesamiento-digital-de-imagenes
Cortés-Osorio, J. A., Chaves-Osorio, J. A., & Mendoza-Vargas, J. A. (2012). Comparación cualitativa y cuantitativa de las técnicas básicas de umbralización local para el procesamiento digital de imágenes. Scientia et Technica, 2(51), 236–241. https://doi.org/https://doi.org/10.22517/23447214.7561
Daroca-Capell, T. (2014). Dimensión y características de los factores que inciden en la contaminación ambiental por residuos sólidos (Tesis de maestría). Universidad de San Martín de Porres. Lima, Perú.
Datapeaker. (2021). Detección de objetos mediante la API de TensorFlow. https://datapeaker.com/big-data/deteccion-de-objetos-mediante-la-api-de-tensorflow/
DataSource.ai. (2020). Comprensión de la Matriz de Confusión y Cómo Implementarla en Python. https://www.datasource.ai/es/data-science-articles/comprension-de-la-matriz-de-confusion-y-como-implementarla-en-python
Díaz-Ramírez, J. (2021). Aprendizaje Automático y Aprendizaje Profundo. Ingeniare. Revista Chilena de Ingeniería, 29(2), 182–183. https://doi.org/http://dx.doi.org/10.4067/S0718-33052021000200180
El Tiempo. (2022). Remueven 4 toneladas de basuras del Canal de Bogotá. https://diarioeltiempo.co/nacional/remueven-4-toneladas-de-basuras-del-canal-bogota/1797/
Elhoseny, M. (2020). Multi-object Detection and Tracking (MODT) Machine Learning Model for Real-Time Video Surveillance Systems. Circuits, Systems, and Signal Processing, 39(2), 611–630. https://doi.org/https://doi.org/10.1007/s00034-019-01234-7
Gil, P., Torres, F., & Ortiz-Zamora, F. G. (2004). Detección de objetos por segmentación multinivel combinada de espacios de color. http://hdl.handle.net/10045/2179
Google. (n.d.-a). Ubicación de la zona del Canal Bogotá que va desde el Centro Comercial las Mercedes hasta el Barrio Cundinamarca. Retrieved October 14, 2023, from https://www.google.com/maps/d/edit?mid=1ZYZvPFaMTUpYFPsmFda_ExxZ8QYWHC4&ll=7.888621594254154%2C-72.50786429021964&z=17
Google. (n.d.-b). Ubicación de la zona del Canal Bogotá que va desde el Centro Comercial Unicentro hasta la Urbanización La Ceiba. Retrieved October 14, 2023, from https://www.google.com/maps/d/edit?mid=1ZYZvPFaMTUpYFPsmFda_ExxZ8QYWHC4&ll=7.909986119363768%2C-72.49815891830148&z=17
Google. (n.d.-c). Ubicación de la zona del Canal Bogotá que va desde el SENA hasta la Diagonal Santander. Retrieved October 14, 2023, from https://www.google.com/maps/d/edit?mid=1ZYZvPFaMTUpYFPsmFda_ExxZ8QYWHC4&ll=7.897297711311962%2C-72.50544728159319&z=17
Hernández-Rodríguez, J. D. (2022). Mejora del modelo de detección de huecos y bolsas de basura basado en deep learning implementado en una Raspberry Pi (en Bogotá, Colombia) (Proyecto final de grado). Universidad de los Andes. Bogotá, Colombia.
La Opinión. (2022, January 6). El canal Bogotá, un basurero fuera de control. La Opinión. https://www.laopinion.com.co/comunidad/el-canal-bogota-un-basurero-fuera-de-control
Majchrowska, S., Mikołajczyk, A., Ferlin, M., Klawikowska, Z., Plantykow, M. A., Kwasigroch, A., & Majek, K. (2022). Deep learning-based waste detection in natural and urban environments. Waste Management, 138, 274–284. https://doi.org/10.1016/j.wasman.2021.12.001
Mery, D. (2004). Visión por Computador. Universidad Católica de Chile.
Ministerio de Ambiente y Desarrollo Sostenible. (2022, May 17). Hoy no se habla de basura, sino de residuos que son insumos para productos: Minambiente. https://www.minambiente.gov.co/asuntos-ambientales-sectorial-y-urbana/hoy-no-se-habla-de-basura-sino-de-residuos-que-son-insumos-para-productos-minambiente/#:~:text=mayo%2017%2C%202022-,Hoy%20no%20se%20habla%20de%20basura%2C%20sino%20de%20residuos%20que,negocio%20a%20partir%20del%20reciclaje.
Moralejo, R., & Storni, A. (2018). Plataforma Detección de objetos en tiempo real. XX Workshop de Investigadores En Ciencias de La Computación (WICC 2018, Universidad Nacional Del Nordeste), 371–375. http://sedici.unlp.edu.ar/handle/10915/67460
Oracle. (n.d.). ¿Qué es la inteligencia artificial (Artificial Intelligence, AI)? Retrieved February 21, 2023, from https://www.oracle.com/co/artificial-intelligence/what-is-ai/
Oracle Developer. (2022). Qué es TensorFlow: una guía completa. https://developer.oracle.com/es/learn/technical-articles/what-is-tensorflow
Pablo G. Bejarano. (2014, August 21). Los últimos avances en reconocimiento de objetos. ThinkBig. https://blogthinkbig.com/reconocimiento-de-objetos/
Ricardo Zapata, J. (2023, November 11). Machine Learning con Scikit Learn. https://joserzapata.github.io/courses/python-ciencia-datos/ml/
Rincon-Ramirez, G., & Baquero-Barreto, C. F. (2022). Método automático computacional para la detección de residuos sólidos en parques (Proyecto final de pregrado). Universidad Católica De Colombia. Bogotá, Colombia.
Salina, M. D. (2021). Deep Learning aplicado al procesamiento de imágenes para la detección de objetos reciclables (Proyecto final de pregrado). Universidad Nacional Arturo Jauretche. Buenos Aires, Argentina.
Secretaría de Cultura, R. y D. (n.d.). ¿Qué es la contaminación ambiental? Retrieved February 21, 2023, from https://www.culturarecreacionydeporte.gov.co/es/bogotanitos/que-es-la-contaminacion-ambiental
Secretaría Distrital de Ambiente. (2021). ¿Sabes qué son los Residuos de Construcción y Demolición (RCD), y cómo disponerlos desde tu casa o empresa? https://www.ambientebogota.gov.co/historial-de-noticias/-/asset_publisher/VqEYxdh9mhVF/content/-sabes-que-son-los-residuos-de-construccion-y-demolicion-rcd-y-como-disponerlos-desde-tu-casa-o-empresa-
Smowltech. (2023). Aprendizaje supervisado y no supervisado: diferencias y similitudes. https://smowl.net/es/blog/aprendizaje-supervisado-no-supervisado/
Stallman, R. (2020). La definición de software libre. Communiars. Revista de Imagen, Artes y Educación Crítica y Social, 3, 151–154.
Tzutalin. (2015). LabelImg. GitHub. https://github.com/HumanSignal/labelImg
Universidad Nacional de Mar del Plata. (2016, April 14). La basura: consecuencias ambientales y desafíos. https://eco.mdp.edu.ar/institucional/eco-enlaces/1611-la-basura-consecuencias-ambientales-y-desafios
Urgilez-Jaramillo, M. V. (2022). Procesamiento digital de imágenes en detección de material contaminante inorgánico en orillas de lagunas (Tesis de maestría). Escuela Superior Politécnica de Chimborazo. Riobamba, Ecuador.
Velázquez-López, N., Sasaki, Y., Nakano, K., MMejía-Muñoz, J., & Romanchik-Kriuchkova, E. (2011). Detección de cenicilla en rosa usando procesamiento de imágenes por computadora. Revista Chapingo Serie Horticultura, 17(2), 151–160. https://www.redalyc.org/articulo.oa?id=60920970007
WWF. (2022, May 17). ¿Por qué seguimos sin reciclar en Colombia? https://www.wwf.org.co/?363591/Por-que-seguimos-sin-reciclar-en-Colombia#:~:text=Si%20no%20separamos%20correctamente%2C%20los,%2D%2C%20o%20en%20la%20naturaleza.