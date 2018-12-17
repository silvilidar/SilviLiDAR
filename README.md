#SilviLiDAR

Script para Qgis que procesa archivos LAZ o LAS para caracterizar las masas forestales, siendo posible evaluar el estado de desarrollo y el momento adecuado para actuar selvícolamente.

Requiere del Software FUSION desarrollado por US Department of Agriculture, Forest Service, Pacific Northwest Research Station. Puede descargarse desde http://forsys.sefs.uw.edu/FUSION/fusion_overview.html
Para trabajar con archivos LAZ requiere LAStools que puede ser descargado desde http://rapidlasso.com/lastools/ y posteriormente copiar el archivo LASzip.dll en la carpeta de instalación de FUSION.

Para instalar SilviLiDAR dentro de Qgis se debe ir al menu Procesos, Caja de herramientas, Scripts, Herramientas, Obtener Scripts a partir de colección de scripts en linea y activar SilviLiDAR.
Para acceder a la herramienta hay que abrir la caja de herramientas desde el menu procesos. A continuación aperecera SilviLiDAR dentro de Scripts, Scripts de usuario.

SilviLiDAR procesa archivos LiDAR en formato LAZ o LAS como los que pueden descargarse de la web del CNIG
http://centrodedescargas.cnig.es/CentroDescargas/buscadorCatalogo.do

Podemos descargar los archivos que necesitemos haciendo una búsqueda por término municipal y guardarlos en una carpeta en el equipo cuya ruta no debe contener espacios en blanco.

Una vez instalado , clicamos dos veces en SilviLiDAR y se nos abrirá una ventana. En ella es imprescindible seleccionar la carpeta en la que se encuentran los archivos LAZ o LAS que queremos procesar.
El resto de campos vienen rellenados por defecto con valores estándar.
Clicamos en Run y se ejecutará el script.

Lo que sucede a continuación es el análisis de los archivos LiDAR mediante el programa FUSION y posteriormente el análisis de cada celda con los parámetros introducidos 
El resultado, que suele tardar unos 2 minutos por cuadricula de 2x2 km, es el siguiente:
· Un shape de polígonos llamado Teselas con los estratos y los posibles tratamientos.
· Otro shape de polígonos llamado claras en el que se ha simplificado el resultado para que pueda emplearse de un modo más cómodo esta información aglutinando las zonas que en las que da clara y tienen una superficie mínima de actuación.
· Otro shape de polígonos llamado resalveo obtenido del mismo modo que el anterior
· Y otro shape de polígonos llamado regeneración donde puede que exista necesidad de cortas de regeneración.
Además se generan en la carpeta de trabajo todos los archivos.
