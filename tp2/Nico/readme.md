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
|Auctions|Cant. de apariciones totales|auctions_total|Nico|-
|Auctions|Cant. de apariciones en la ultima hora|auctions_last_hour|Nico|-
|Auctions|Tiempo medio entre apariciones|secs_to_next_mean|Nico|-
|Auctions|Tiempo desde ultima aparicion|secs_since_last_arrival|Nico|
|Auctions|Cuantas veces aparecio el 20 o 21|amount_auctions_in_weekend|Nico|-
|Auctions|Ultimo dia de la ventana es  weekend|is_last_weekend|Nico|-
|Auctions|Se realizó subastan entre [0,2] hs|alta_demanda|Lucas|-
|Auctions|Ponderación respecto a horarios|pond_hora_ext|Lucas|-
|Auctions|Aparecio el fin de semana?|appears_on_weekend |Manu|-
|Events|Cant. de cada evento|amount_events|Manu|-
|Events|Ultimo evento|last_event (y los que no tienen events?)|Manu|-
|Events|Ultimos eventos fueron con wifi?| wifi | Manu |-
|Events|Secuencia de n eventos|-|-|-
|Installs|Cant. de Apps distintas instaladas|count_app_dif|Lucas|-
|Installs|Lista de equipos con mas instalaciones y  si device pertenece|-|-|-
|Installs|Instaló en la ventana anterior|win_2_in_1,win_3_in_2|Lucas|-
|Installs|Cantidad de clicks por evento|-|-|-
|Installs|Una vez armado los features, cuantos K vecinos instalaron|-|-|-
|Clicks|Armar dimensiones de device y ver cuarto donde tiende a hacer clicks|-|-|-
|Clicks|Cantidad de Advertisers que los tiene|amount_dif_advertisers|Manu|-
|Clicks|Tiempo promedio de clicks|timeToClick_mean |Manu|-
 
