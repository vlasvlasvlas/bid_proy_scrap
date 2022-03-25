# bid_proy_scrap

## Objetivo
El objetivo del script es la generación en formato deutilizable xlsx/csv de la información de proyectos y operaciones de prestamos BID por país.

Para esto se utiliza un proceso de scrapeo de datos html cuyo origen es el listado de proyectos BID por país.

## Requerimientos
- Python 3
- Extensiones Pandas, BeautifulSoup


## Proceso
- Toma listado de id de proyectos de proyectos_lista.csv
- Itera por cada fila, recreando la url del proyecto. Por cada url:
	- utiliza beautifulsoup para extración scrap de los tags de project-field-title y project-field-data del sitio
	- almacena pares es diccionario
- Pasa total de resultados a un pandas DataFrame y exporta resultado en xlsx/csv

## To-Do
- Traer url xlsx de listado de proyectos, pensando en uno o varios países (latam?)

