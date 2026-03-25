# Curso de Devops con Docker de la universidad de Helsinki

## Comandos

### Dockerfile

#### Construir una imagen

- -f: Agrega un nombre de archivo para el Dockerfile

```bash
$ docker image build -t <nombre-imagen> <contexto>
```

```bash
$ docker build -t <nombre-imagen> <contexto>
```

### Imagen

#### Listar todas las imagenes

```bash
$ docker image ls
```

#### Eliminar una imagen

```bash
$ docker image rm <nombre-imagen>
```

#### Elimina las imagenes no utilizadas

```bash
$ docker image prune
```

#### Buscar una imagen

```bash
$ docker search <término>
```

#### Descargar una imagen

```bash
$ docker image pull <nombre-imagen>
```

```bash
$ docker pull <nombre-imagen>
```

#### Crear un nuevo tag referenciando otra imagen

```bash
$ docker image tag <src:tag> <dst:tag>
```

```bash
$ docker tag <src:tag> <dst:tag>
```

### Contenedor

- docker run
    - -i: interactive
    - -t: tty
    - -d: detached
    - --rm: remove
    - -v: attach a volume or a bind mount
    - -p: connect a port in the host to a port in a container

#### Ejecutar un contenedor desde una imagen

```bash
$ docker container run <nombre-imagen>
```

```bash
$ docker run <nombre-imagen>
```

#### Ejecutar un contenedor desde una imagen sin retener la terminal

```bash
$ docker run -d <nombre-imagen>
```

#### Ejecutar un tty en un contenedor

```bash
$ docker run -it <nombre-imagen>
```

#### Ejecutar un contenedor y eliminarlo al detenerlo

```bash
$ docker run --rm <nombre-imagen>
```

#### Pausar un contenedor

```bash
$ docker container pause <nombre-contenedor>
```

```bash
$ docker pause <nombre-contenedor>
```

#### Reaunudar un contenedor pausado

```bash
$ docker container unpause <nombre-contenedor>
```

```bash
$ docker unpause <nombre-contenedor>
```

#### Adjuntar a un contenedor en ejecución

```bash
$ docker container attach <nombre-contenedor>
```

```bash
$ docker attach <nombre-contenedor>
```

- --no-stdin: no le asgina el STDIN al contenedor

#### Detener un contenedor

```bash
$ docker container stop <nombre-contenedor>
```

```bash
$ docker stop <nombre-contenedor>
```

#### Detener forzadamente un contenedor

```bash
$ docker container kill <nombre-contenedor>
```

```bash
$ docker kill <nombre-contenedor>
```

#### Comenzar un contenedor detenido

```bash
$ docker container start <nombre-contenedor>
```

```bash
$ docker start <nomber-contenedor>
```

#### Listar los contenedores en ejecución

```bash
$ docker container ls
```

```bash
$ docker ps
```

#### Lista todos los contenedores, incluso los finalizados

```bash
$ docker container ls -a
```

#### Ver los logs de un contenedor

```bash
$ docker container logs <nombre-contenedor>
```

```bash
$ docker logs -f <nombre-contenedor>
```

#### Ejecuta un comando en un contenedor en ejecución

```bash
$ docker container exec <nombre-contenedor> <comando>
```

```bash
$ docker exec <nombre-contenedor> <comando>
```

#### Copiar archivos entre el filesystem local y un contenedor

```bash
$ docker container cp <src> <dst>
```

```bash
$ docker cp <src> <dst>
```

#### Ver la diferencia de los archivos en un contenedor

```bash
$ docker container diff <nombre-contenedor>
```

```bash
$ docker diff <nombre-contenedor>
```

#### Crea una nueva imagen a partir de un contenedor

```bash
$ docker container commit <nombre-contenedor> <nombre-imagen>
```

```bash
$ docker commit <nombre-contenedor> <nombre-imagen>
```

#### Eliminar un contenedor

```bash
$ docker container rm
```

```bash
$ docker rm
```

#### Elimina los contenedores detenidos

```bash
$ docker container prune
```
