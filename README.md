![DANELOGO](Figuras/dane_logo.PNG)
 
 # Percepción de Discriminación [Mintic]

La medición de la percepción de la confianza en el instituto nacional de estadísticas se enmarca en el propósito de la  (OCDE, 2017) de fortalecer las estadísticas oficiales para la medición del capital social, como parte de un sistema robusto para la comprensión y medición del bienestar. Surgió como respuesta a la Iniciativa de Paris 21 promueve la medición de la confianza de los ciudadanos en los institutos nacionales de estadísticas, los sistemas estadísticos nacionales y las estadísticas oficiales. La confianza en las estadísticas, según (PARIS 21, 2019) se entiende como la credibilidad en los productos estadísticos producidos en el Sistema Estadístico Nacional, el cual actúa como un proveedor de formación estadística creíble, precisa y oportuna libre de interferencia política inapropiada. 
En este sentido, el objetivo del proyecto es medir la percepción y confianza que tienen los usuarios de Twitter frente al DANE y a los productos estadísticos, a través del uso de fuentes alternativas para la captura de datos y el diseño e implementación de técnicas y metodologías de procesamiento de lenguaje natural y análisis de sentimientos.
La información estadística derivada de este proyecto contribuye a conocer la percepción de los diferentes usuarios en las estadísticas producidas por el DANE, desagregada a nivel geográfico, así como conocer quiénes son los usuarios más activos en Twitter, los temas más recurrentes y cuál es la polaridad de sus opiniones, y aspectos como la relación de esta percepción con las diferentes publicaciones del DANE, lo cual puede contribuir a la gestión de la difusión y la cultura estadística en el DANE. 
Este repositorio contiene las bases de datos de los Tweets publicados por DANE_Colombia, desde octubre de 2020 hasta enero de 2021, descargados mediante técnicas de web scraping mediante el [API de Twitter](https://developer.twitter.com/en/docs/twitter-api), así como los diccionarios de datos de estas bases. Este ejercicio exploratorio se desarrolla como uno de los proyectos de la línea de aprovechamiento de fuentes de información alternativas (Twitter) de la Coordinación de Prospectiva y Analítica de Datos de la Dirección de Regulación, Planificación, Estandarización y Normalización (DIRPEN) del DANE.

## Contenido

1. [Tecnologías usadas](#tecnologías)
2. [Piloto DataSandbox](#piloto)
3. [Datasets](#datasets)
4. [Diccionarios](#diccionarios)
5. [Dashboard](#dashboard)

## Tecnologías usadas

Este ejercicio fue desarrollado utilizando el servicio de computación en la nube creado por Microsoft, [Microsoft Azure](https://azure.microsoft.com/es-es/). En adición, se utilizaron las plataformas [Databricks](https://databricks.com/) y [Google Drive](https://www.google.com/intl/es_co/drive/) así como los lenguajes de programación [Python](https://www.python.org/).

De igual manera se usaron las siguientes librerías:

Python
- Pandas
- Plotly
- facebook_scraper



## Dashboard

En la ubicación [`App/Despligue`](App/Despligue) se encuentra tanto el Notebook ``dashboard_dev_dane.ipynb`` como el modelo de dashboard ``dashboard_percepciondisc_dane.html`` desarrollados para este ejercicio exploratorio con información referente al conjunto de datos ``cwg.csv``.
