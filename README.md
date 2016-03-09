# DOCKER XAMP:

Descargar e instalar Docker ToolBox
```sh
https://www.docker.com/products/docker-toolbox
```

#### OBSERVACIONES:
Se recomienda crear un docker-machine independiente para el proyecto
```sh
$ docker-machine create -d virtualbox MY_DOCKER
```
Verificar la reación de MY_DOCKER
```sh
$ docker-machine ls
```
Seleccionar "MY_DOCKER" como maquina de trabajo
```sh
$ eval $(docker-machine env MY_DOCKER)
```
Verificar que "MY_DOCKER" este seleccionado (aparece un '*' al lado de su nombre)
```sh
$ docker-machine ls
```


### BUILD:

```sh
$ docker-compose build
$ docker-compose up -d
```

### TESTING:
Verificar si el docker está corriendo
```
$ docker-compose ps
```


* "XXX" de la ip varía dependiendo de la VM (100, 101, 102...)

CARPETA WWWW
> 192.168.99.XXX:41062/www

SSH
```
$ ssh root@192.168.99.XXX -p 41061
> pass : root
```

### STOP:

```sh
$ docker-compose stop
```

=)
