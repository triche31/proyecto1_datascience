
# Proyecto 1 del Bootcamp en Data Science: Proceso ETL de una API

En este proyecto el objetivo que tenemos es el de hacer un proceso de ETL: extracción, transformación y carga.

Lo hacemos a través de llamadas a la API de la red eléctrica española: https://apidatos.ree.es/es/datos/

Nos resultaba complicado tener las regiones con sus correspondientes estructuras, (si es la zona peninsular, si es a nivel de comunidad autónoma, si se trata de Canarias, Baleares,
Ceuta o Melilla) y los códigos que tenemos en la web de la ree, por ello nos copiamos la información y lo pasamos a un excel, que es el fichero que aquí se encuentra con el nombre de Regiones.xlsx

Las llamadas a la API las hemos realizado con la librería requests. También hemos utilizado pprint y json para ver la estructura de los datos de un forma más amigable.

Los datos obtenidos están bastante limpios por lo que la parte de limpieza es bastante básica, entre las cosas que hicimos está: la eliminación de nans, cambio de formatos de los datos y eliminación de las columnas que no consideramos relevantes para trabajar con los diferentes DataFrames.

No hay mucha información en la web de ree de cómo hay que utilizar la API, por lo que a base de investigar los parámetros y lo que significan sacamos lo que nosotras considerábamos importante para este proyecto.

La ultima parte, la de carga, la hacemos a través de airtable, y para ello realizamos una función que nos permita subir toda la información, sin el limitante que posee dicha API.
También hacemos lo contrario, una función para descargar esos datos en caso de que los necesitemos.

Por ultimo, tenemos una serie de visualizaciones realizadas con matplotlib y seaborn que nos parecían interesantes comentar como puede ser la evolución de la energia renovable.


### Desafíos

El primer desafío con el que nos encontramos sin duda fue la falta de documentación que hay sobre esta API en concreto, pues cuando accedes a su web tienes poca información y apenas indican que hace cada componente para formar el request.

A continuación, teníamos una lista de regiones que queríamos utilizar pero no teníamos cómo hacerlo, y al final optamos por hacerlo como hemos indicado más arriba.

Además, la información proporcionada por la API estaba organizada en forma de listas de diccionarios con diccionarios y diccionarios, lo cual nos complicaba acceder a los datos de forma sencilla. 

Una vez que teníamos todos los dataframes, debíamos de subirlo a Airtalbe y ahí tuvimos problemas e indiscrepancias con los formatos de las columnas entre Airtable y nuestro data.


### Evolución de energía renovable y no renovable 



![image](https://github.com/triche31/proyecto1_datascience/assets/155429359/8b293b24-5aff-4f9d-afb1-a78d4db82c08)


## Authors

- [@Esthergg93](https://www.github.com/Esthergg93)
- [@e-velazco](https://www.github.com/e-velazco)


