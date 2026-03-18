# Curso de Devops con Docker de la universidad de Helsinky

## Comandos

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

#### Descargar una imagen

```bash
$ docker image pull <nombre-imagen>
```

```bash
$ docker pull <nombre-imagen>
```

### Contenedor

- docker run
    - -i: interactive
    - -t: tty
    - -d: detached
    - --rm: remove

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
