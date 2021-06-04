# Análisis

A continuación puedes encontrar el análisis del proyecto en una presentación:

[Slides](https://docs.google.com/presentation/d/1WKOwHYLG778pwL1FK-Veewb35lU5mFCER7uFjNl4GkE/edit?usp=sharing)

# Requerimientos

1. Anaconda
2. Descargar los datasets alojados en [kaggle](https://www.kaggle.com/datasnaek/youtube-new?).
3. Ubicar los datasets en el root de este proyecto.
4. Ejecutar el notebook

# Herramientas

- Jupyter notebooks

### Librerías
- Pandas
- Numpy
- MATPLOTLIB
- SEABORN
- Datetime
- Altair
- JSON

### Lenguajes

- Python


<!-- # LISTADO DE TEORÍAS Y CONCEPTOS QU FUERON UTILIZADOS PARA LLEGAR A LAS RESPUESTAS -->

# Conceptos

1. Procesamiento de datos y librerías para ciencia de datos, en esta prueba se tomaron dos que son Numpy y Pandas

2. Procesamiento de archivos:
    - Gestión de archivos CSV
    - Gestión de archivos JSON

3. DataFrames:
    - Funcionamiento con la librería Pandas
    - Obtención de series, columnas, selección de múltiples columnas/filas, indices.
    - Funciones para operar dentro de un DataFrame, como por ejemplo: **.head, .describe, .tail, .copy, .columns, .unique** entre otras que se reflejan en el código. 
    - Agrupaciones de datos con la función **groupby**
    - Borrado de filas y columnas (**.drop**, Conocer los parámetros axis, si es para filas se utiliza 0 y si es para columnas 1)
    - Gestión de nulos (funciones como **.isnull, .fillna, .dropna**)

4. Estructura de datos
    - Diccionarios

5. Procesamiento de datos y visualización con Python
    - Implementación de gráficas dependiendo de los requerimientos y objetivos
    - MATPLOTLIB
    - SEABORN

6. Calidad de los datos:
    - Identificación de los datos necesarios para realizar analisis que den valor al dato
    
7. Preparación y pre proceso de datos:
    - Limpieza de los datos:
    - Estandarizaron de formatos
    - Feature engineering
    - Agregación y relativización

8. Análisis descriptivo (comprender las relaciones que existen entre los datos):
    - Existencia de patrones y regularidades de los fenómenos estudiados 
    - Análisis de correlación en esta prueba se realizo la correlación entre vistas y likes de cada país
    - Sumarización y descripción estadística de los datos
    - "slice and dice"
    - Análisis de clusterización
    - Detección de anomalías

# Decisiones Técnicas

Elegir que librerías importar o que gráficas utilizar, que tipo de modelos se necesitan dependiendo de las variables que se tengan. 

 - **Análisis DataFrame**: Tras ver cada uno de los Dataset quería realizar el análisis a cada país por separado, para tener una visión mas amplia de lo que pasaba con cada país por individual ya que en el enunciado de la prueba dice que se quiere entrenar youtubers para diferentes culturas, y como ya sabemos cada país es una cultura muy distinta y cada uno de ellos busca características diferentes y también analizarlo por continentes para llegar a ver eso que no es visible a simple vista. 
 
- **Herramientas Visualización**:
En cuanto a la parte técnica utilice herramientas que me permitieran extraer los datos de forma eficiente y rápida y en la parte de visualización me enfoque en que cada grafica mostrara de forma correcta los datos que quería representar, estas librerías de visualizaciones se desarrollan de forma sistemática. 

- **Seaborn**: Es una librería que me gusta mucho porque actúa como un interfaz de alto nivel sobre Matplotlib y se utiliza menos código y quería  mostrar distribuciones en una nube de puntos con dos variables y también que me mostrar una regresión lineal en nube de puntos y eso me lo permitía esta librería.

- **Contenido Viral**: Se tomaron en cuenta las medias de los **views, likes, comments_count** ya que este tipo de contenido no se puede analizar solamente con las vistas. 

- **Contenido Polémico**: Se tomo en cuenta las vistas ya que para este tipo de video no son de preferencia de las personas sino que generen intriga. 

- **Contenido Especifico**: Elegí realizarlo con la categoría de film & animation ya que viendo las gráficas de contenido viral y contenido polémico, se pudo observar que esta categoría la mayoría de las veces se encuentras entre los 5 - 7 primeros puestos.

## Siguientes Pasos

1. Realizar un modelo predictivo para el país de preferencia, donde se muestre la predicción de días que se puede demorar un video en hacerse trending

2. Predecir la cantidad de likes de un video, tras días después de volverse trending