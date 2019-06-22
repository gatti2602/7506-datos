Ideas
-----

* Usar KNN para asignar prob de que convierta
* Usar neuronas para campos numericos
* Arboles de decision para regresion final

Dado que: 
1. Events se asocia con Installs mediante event_uuid
2. Events, Installs y Clicks estan asociados por trans_id

Se puede: 
* Determinar el evento anterior al install
* Descartar el evento anterior y obtener los n eventos anteriores
* Buscar secuencias que hayan llegado a estos eventos



---
Features posibles 
-----------------

|Dataframe|Feature|Implementado en Col.|Implementado Por|Funciona?|
|---------|-------|--------------------|----------------|---------|
|Auctions|Cant. de sources distintos que tienen el dispositivo|amount_dif_src |Manu|-
|Auctions|Cant. de apariciones totales|auctions_total (En curso)|Nico|-
|Auctions|Cant. de apariciones en la ultima hora|auctions_last_hour (en curso)|Nico|-
|Auctions|Tiempo medio entre apariciones|(En curso)|Manu|-
|Auctions|lambda de una exponencial en los tiempos de un usuario|-|-|-
|Auctions|Tiempo desde ultima aparicion|secs_since_last_arrival|Nico|
|Auctions|Cuantas veces aparecio el 20 o 21|-|-|-
|Auctions|Aparecio el fin de semana?|-|-|-
|Events|Cant. de cada evento|-|-|-
|Events|Ultimo evento|-|-|-
|Events|Ultimos eventos fueron con wifi?|-|-|-
|Events|Secuencia de n eventos|-|-|-
|Installs|Cant. de Apps distintas instaladas|-|-|-
|Installs|Lista de equipos con mas instalaciones y  si device pertenece|-|-|-
|Installs|Instaló en la ventana anterior|-|-|-
|Installs|Cantidad de clicks por evento|-|-|-
|Installs|Una vez armado los features, cuantos K vecinos instalaron|-|-|-
|Clicks|Armar dimensiones de device y ver cuarto donde tiende a hacer clicks|-|-|-
|Clicks|Cantidad de Advertisers que los tiene|-|-|-
|Clicks|Tiempo promedio de clicks|-|-|-
