# Proyeto EmergencIAs - Activaciones Madrid SAMUR-PC

Este proyecto se ha realizado como proyeto final del Máster en Data Science de MIOTI. Esta basado en las Activaciones de SAMUR - PROTECCIÓN CIVIL de la ciudad de Madrid.

## Contenido y Estrutura del proyecto
El proyeto se divide en 5 notebooks y 2 carpetas **datos** e **img**:

* **Emergencias_Cluster.iypnb**  -  En este notebook es donde se encuentra el modelo no supervisado de clasterización basado en un algoritmo jerárquico aglomerativo.
* **Emergencias_Modelo.iypnb**  -  En este notebook es donde están los modelos para la predicción de tiempos de respuesta, tanto con un enfoque de regresión como con un enfoque de clasificación.

* **Emergencias_Pre.iypnb**  -  En este notebook es donde están todas las labores de preprocesamiento que se han llevado acaba. Entre ellos la reconsturcción de la serie temporal, así como la alineación con los nombres oficales de cada uno de los distritos.

* **emergencias_prophet.iypnb**  -  En este notebook es donde están todas las previsiones lanzadas copn Facebook Prophet. También están la creación de los distintos calendarios de holidays, así coomo la instaciación de los festivos nacionales de España.

* **Emergencias_Vis.iypnb**  -  En este notebook es donde están la mayoría de las visualizaciones de datos, tato en gráficos de barras, series temporales, así como el mapa cloropéctico de la ciudad de Madrid y sus 21 distritos de la ciudad de Madrid. 

* **Emergencias_Vis.iypnb**  -  En este notebook es donde están la mayoría de las visualizaciones de datos, tato en gráficos de barras, series temporales, así como el mapa cloropéctico de la ciudad de Madrid y sus 21 distritos de la ciudad de Madrid. 

### Carpeta "datos"
En esta carpeta residen los ficheros de datos:
* **activaciones_samur_2017.csv** - Activaciones de SAMUR-PC del 2017
* **activaciones_samur_2018.csv** - Activaciones de SAMUR-PC del 2018
* **activaciones_samur_2019.csv** - Activaciones de SAMUR-PC del 2019
* **activaciones_samur_2020.csv** - Activaciones de SAMUR-PC del 2020
* **activaciones_samur_2021.csv** - Activaciones de SAMUR-PC del 2021
* **distritos.geojson** - Datos geográficos de los 21 distritos de la ciudad de Madrid.
* **emergencias_pp.csv** - Fichero intermedio de preprocesamiento.
* **emergencias_pp_def.csv** - Fichero definitivo de la fase de preprocesamiento general.
* **emergencias_reg.csv** - Fichero con el resultado de las distintas tareas realizadas de Feature engineering para el modelo de regresión y clasificación de tiempos respuesta.
* **prediccion_2022.csv** - Fichero con las previsiones realizadas por prophet para el 2022 y que tiene la estructura para poder ser procesado y visualizado en el mapa cloropéctico de la ciudad de Madrid.
### Carpeta "img"
Imagenes utilizadas en los notebooks.


## Datos

* [Portal datos abiertos Ayuntamiento Madrid. Activaciones SAMUR-PC](https://datos.madrid.es/sites/v/index.jsp?vgnextoid=50d7d35982d6f510VgnVCM1000001d4a900aRCRD&vgnextchannel=374512b9ace9f310VgnVCM100000171f5a0aRCRD)
* [Datos geográficos Distritos de Madrid](https://team.carto.com/u/jsanz/tables/distritos/public)

## Principales librerias utilizadas.

* **pandas**
* **numpy**
* **matplotlib**
* **geopandas**
* **geoplot**
* **folium**
* **shapely**
* **contextily**
* **pyproj**
* **sklearn**
* **scipy**
* **fbprophet**
