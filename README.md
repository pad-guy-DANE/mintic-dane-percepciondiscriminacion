![DANELOGO](Figuras/dane_logo.PNG)
 
# Percepción de Discriminación [Mintic]

El DANE, como coordinador del Sistema Estadístico Nacional (SEN), busca impulsar la innovación en la producción y difusión de las estadísticas oficiales y en el uso estadístico de registros administrativos y, en esa medida, viene trabajando desde hace algunos años en algunos proyectos que propenden por el uso de fuentes y metodologías secundarias para el análisis de los datos.
Dentro de estos proyectos se encuentra la Medición de los indicadores ODS 16.b.1. Proporción de la población que declara haber experimentado personalmente discriminación o acoso en los últimos 12 meses por un motivo de discriminación prohibido por el derecho internacional de los derechos humanos y 16.7.2 Proporción de la población que cree que la toma de decisiones es inclusiva y receptiva, por sexo, edad, discapacidad y grupo de población, a través de redes sociales (Facebook y Twitter).

En términos generales, la metodología responde a un problema clásico de procesamiento de lenguaje natural (PLN), es decir que para un conjunto de datos dado se identificó si los datos están relacionados con algún tema. Se empleó un análisis semisupervisado, en el que se definen los términos de búsqueda y se busca en el conjunto de datos para identificar estos términos y los correlacionados con ellos. Luego se construyó un modelo que "aprendiera" a identificar esos conceptos en determinados contextos y los asociara con la discriminación. Posteriormente, se contrastará con un análisis supervisado basado en comentarios etiquetados por marcadores humanos.

Para el desarrollo de este proyecto el DANE viene recibiendo el apoyo de la iniciativa D4N, codirigido por la División de Estadística de las Naciones Unidas, el Banco Mundial, la Asociación Mundial para los Datos sobre el Desarrollo Sostenible y la Red de Soluciones para el Desarrollo Sostenible, la cual tiene como objetivo apoyar a los países en el uso de fuentes, tecnologías y métodos innovadores para la producción y difusión racionalizada de datos mejores, más oportunos y desglosados para el desarrollo sostenible, en sintonía con los postulados misionales del DANE como coordinador del SEN.
Asimismo, el DANE ha contado con un acompañamiento para la definición del marco conceptual por parte de la Consejería Presidencial para los Derechos Humanos (CPDAI).
El equipo de trabajo del DANE continuará avanzando en 	la profundización de la visualización de los resultados, la exploración de otros modelos para contrastar los resultados de esta versión preliminar y el desarrollo de estrategias para garantizar la calidad de la recogida, el tratamiento y el análisis de los datos.

## Contenido

1. [Tecnologías usadas](#tecnologías)
2. [Datasets](#datasets)
3. [Dashboard](#dashboard)

<!--- 
2. [Piloto DataSandbox](#piloto)
4. [Diccionarios](#diccionarios)
-->

## Tecnologías usadas

Este ejercicio fue desarrollado utilizando el servicio de computación en la nube creado por Microsoft, [Microsoft Azure](https://azure.microsoft.com/es-es/). En adición, se utilizaron las plataformas [Databricks](https://databricks.com/) y [Google Drive](https://www.google.com/intl/es_co/drive/) así como los lenguajes de programación [Python](https://www.python.org/).

De igual manera se usaron las siguientes librerías:

Python
- Pandas
- Plotly
- facebook_scraper


## Datasets

Se encuentran dos bases de datos principales (ubicadas en [`Datos-Ejemplo/Para-Modelo`](Datos-Ejemplo/Para-Modelo)):

* ``popular_posts_categories.rar`` <br>
Este archivo, consta de 10 carpetas correspondientes a posts de perfiles públicos de Facebook organizados en categorías.

* ``popular_base.rar`` <br>
Este archivo, consta de 42 bases correspondientes a comentarios asociados a posts de 36 perfiles públicos de Facebook.

En adición, se encuentra una base de datos (ubicada en [`Datos-Ejemplo/Procesados`](Datos-Ejemplo/Procesados)):

* ``cwg.part01.rar`` y ``cwg.part02.rar`` <br>
Esta base consta de 771502 registros, correspondientes a posts y sus comentarios asociados para los, junto con preprocesamiento de texto de post y de comentario.

## Dashboard

En la ubicación [`App/Despligue`](App/Despliegue) se encuentra tanto el Notebook ``dashboard_dev_dane.ipynb`` como el modelo de dashboard ``dashboard_percepciondisc_dane.html`` desarrollados para este ejercicio exploratorio con información referente al conjunto de datos ``cwg.csv``.
