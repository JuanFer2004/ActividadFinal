# Análisis de datos MovieLens con Apache Spark

## Descripción del proyecto

Este proyecto tiene como objetivo realizar un análisis exploratorio de datos utilizando Apache Spark sobre el dataset MovieLens. El trabajo permite procesar, limpiar, analizar y visualizar información relacionada con películas, usuarios, calificaciones y tendencias de valoración.

El análisis se desarrolla en un notebook de Python, aplicando Spark para el manejo eficiente de grandes volúmenes de datos y comparando su utilidad frente a métodos tradicionales de procesamiento.

## Dataset utilizado

El conjunto de datos utilizado corresponde a MovieLens Latest, disponible en el siguiente enlace:

https://files.grouplens.org/datasets/movielens/ml-latest.zip

Este dataset contiene información sobre:

- Películas
- Calificaciones de usuarios
- Géneros cinematográficos
- Etiquetas asignadas por usuarios
- Fechas de interacción

Los archivos principales utilizados son:

- `ratings.csv`: contiene las calificaciones realizadas por los usuarios.
- `movies.csv`: contiene información de las películas y sus géneros.
- `tags.csv`: contiene etiquetas asignadas por usuarios.
- `links.csv`: contiene identificadores externos de películas.

## Objetivo general

Analizar el comportamiento de las calificaciones de películas en MovieLens mediante Apache Spark, identificando patrones relevantes en los datos y generando visualizaciones que permitan interpretar los resultados obtenidos.

## Objetivos específicos

- Cargar el dataset MovieLens en un entorno Spark.
- Realizar limpieza de datos eliminando duplicados, valores nulos y registros inválidos.
- Transformar variables temporales para facilitar el análisis por año.
- Generar consultas y agregaciones con Spark SQL.
- Crear visualizaciones para interpretar tendencias de calificación, géneros y comportamiento de usuarios.
- Comparar el rendimiento del procesamiento con Spark frente a métodos tradicionales.

## Tecnologías utilizadas

- Python
- Apache Spark
- PySpark
- Spark SQL
- Pandas
- Matplotlib
- Jupyter Notebook / Google Colab

## Proceso desarrollado

### 1. Carga de datos

Se cargaron los archivos principales del dataset MovieLens en DataFrames de Spark, permitiendo trabajar con grandes volúmenes de datos de manera distribuida.

### 2. Limpieza de datos

Se eliminaron registros duplicados y valores nulos en columnas clave como `userId`, `movieId`, `rating` y `timestamp`. También se validó que las calificaciones estuvieran dentro del rango permitido de 0.5 a 5.0.

Además, el campo `timestamp` fue transformado a una fecha legible para realizar análisis temporales.

### 3. Análisis exploratorio

Se realizaron consultas para identificar:

- Distribución de calificaciones.
- Películas con mayor número de valoraciones.
- Promedio de calificación por película.
- Tendencias de calificación por año.
- Comportamiento general de los usuarios.

### 4. Visualizaciones

El proyecto incluye cinco visualizaciones, cada una compuesta por:

- Markdown de análisis.
- Código de generación del gráfico.
- Visualización gráfica.
- Markdown de interpretación.

Estas visualizaciones permiten comprender mejor los patrones presentes en el dataset.

## Visualizaciones incluidas

1. Distribución de calificaciones en MovieLens.
2. Películas con mayor número de valoraciones.
3. Promedio de calificación por película.
4. Evolución temporal de las calificaciones.
5. Análisis adicional sobre géneros o comportamiento de usuarios.

## Conclusiones

El análisis permitió evidenciar que las calificaciones en MovieLens tienden a concentrarse en valores altos, especialmente entre 3.0 y 5.0. También se identificaron películas con alta participación de usuarios y patrones temporales relevantes en las valoraciones.

El uso de Apache Spark facilitó el procesamiento eficiente del dataset, demostrando su utilidad para trabajar con grandes volúmenes de información. Sin embargo, también se identificaron limitaciones relacionadas con la configuración inicial del entorno y la necesidad de convertir algunos resultados a Pandas para su visualización.

## Cómo ejecutar el proyecto

1. Descargar el dataset desde:

   https://files.grouplens.org/datasets/movielens/ml-latest.zip

2. Descomprimir el archivo ZIP.

3. Cargar los archivos CSV en el entorno de trabajo.

4. Ejecutar el notebook paso a paso.

5. Revisar los resultados, gráficos e interpretaciones generadas.

## Autor

Proyecto desarrollado por:

Julian Camilo Cardena Torres -
Juan Fernando Bueno Torres

