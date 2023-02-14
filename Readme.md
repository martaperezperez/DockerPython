# Docker + Python

----

# Creamos un contenedor sencillo de python

`$ docker run -it -rm -v "$PWD":/usr/src/myapp python:3 python script.py`
`docker` el comando base, es el daemon
`run` crear el comando
`-it` dos opciones que me valen para interactuar con la terminal del contenedor
`--rm`  borrar el contenedor cuando finaliza la accion
`-v`  define el mapeo del volumen a continuaciobn
`"$SPWD":` el directorio donde estamos
`usr/src/myapp` el direcctorio dentro del contenedor
`-w` el direcctorio de trabajo (workdir)
`python:3` la imagen de la que se creara el contenedor
`python script.py` el script que debe ejecutarse en el contenedor

Para ejecutar un script de python con el cpomando , debemos darle la ultima opcion:

$ docker run -it --rm -v "$PWD":/usr/src/myapp -w /usr/src/myapp python:3 python main.py