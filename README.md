# Parcial_Paralela
Programas que se usaron en el desarrollo del experimento
Makefile: Se conoce el archivo cabecero, que crea los objetos y ejecutables para el funcionamiento de los benchmark
lanzador.pl: El lanzadar es el archivo ejecutor, en el cual se le asigna las cargas y repeticiones de los benchmark,
además de que llama uno por uno a estas clases de juguete para evaluar el rendimiento.
mm_lib.c: Se encarga de tener el procedimiento de las funciones, listas para ser ejecutadas.
mm_lib.h: Es el puente que conecta las librerias con los programas que la llamen.
mm_main_double.c: Es el benchmark de matrices con datos double.
mm_main_double_rnd.c: Es el benchmark de matrices con datos aleatorios de tipo double.
mm_main_int.c: Es el benchmark de matrices con datos enteros.
mm_main_int_rnd.c: Es el benchmark de matrices con datos aleatorios de tipo enteros.

Para descargar los programas y posteriormente ejecutarlos, se debe de desplegar las opciones de la pestaña 'code' y seleccionar
la opción de download zip. Hecho lo anterior, se procede a extraer la carpeta generada por github.

Para correr independientemente cada programa, mediante la terminal se debe realizar una limpieza con el comando 'make clean' (esto se debe hacer si se encuentran objetos generados),
después con el comando 'make all', se generaran los objetos y ejecutables de cada programa y con el comando './(nombre del programa) (tamaño de la matriz) se ejecutara cada programa.

Si el deseo del servidor es ejecutarlos todos al mismo tiempo, se debe realizar el mismo proceso previo de los comandos 'make clean' y 'make all', y mediante la terminal
se debe de escribir './lanzador.pl', hecho esto, se ejecutaran los 4 benchmarks con los parametros establecidos dentro del fichero lanzador.pl

Nota: Se debe tener presente que si se ejecuta el lanzador, se ejecutaran los 4 benchmarks con 30 repeticiones por carga cada uno.
