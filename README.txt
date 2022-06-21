Tarea Scrapy (Tokens Vs Vocabulario)

Descripcion: Scrapy a listado de links de Wikipedia que van asociados a articulos de contenido variado asociados a arquitectura, arqueología y arte, coloconadole un limite de 25 links. estan clasificados en una unica categoria en la cual se extrae el titulo del articulo y el primer parrafo del mismo.

Contribuciones: Jorge Cardona: Generacion de código , identificación de estructura de página Celmy Rojas:Generacion de código , funcion de callback para llamar a cada link Marvin Gutierrez: Generacion de código, generación de archivo csv Marlon Fuentes: Generacion de código,documentación y almacenamiento de la información ( YIELD)

Información Adicional: El objetivo principal es recopilar el titulo y primer párrafo de cada artículo, se notó que la mayoria de veces estos parrafos terminan en punto (.) o espacion en blanco. Por lo que se utilizaron esos caracteres como caracteres de corte de línea y en caso los parrafos no terminaran en esas 2 condiciones se optó por cortar el scrapping a los 25 caracteres recopilados.

conda create -n environment_tarea1

conda activate environment_tarea1

conda activate scrapping conda install scrapy -c conda-forge

scrapy startproject wikipedia_scraping

Ejecutar este comando para generar csv con información de :

titulo: titulo de cada link
parrafo: primer parrafo de cada link
scrapy runspider Wiki.py -o data.csv
PARA EJECUCIÓN:

abrir un pompt
colocarse en la ruta de la carpeta spider
ejecutar el siguiente comando para que corra: scrapy runspider Wiki.py -o data1.csv  *poner data2 y data3 para generar los proximos archivos
En caso se genere algun conflicto tambien se puede utilizar la opcion: scrapy crawl Wiki -o data1.csv *poner data2 y data3 para generar los proximo archivos

En la Carpeta Tarea2 los archivos vienen incluidos para ser cargados en el Jupiter Notebook.

Jupyter Notebook. 

En la carpet Tarea2 vienen incluidos los archivos data1, data2 y data3 los cuales puedes utilizar para cargarlos en el Jupyter Notebook y especificar la direccion de los archivos. 

Luego solo debes darle play a cada seccion para ir ejecutando el codigo. 