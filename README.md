# Curso de Devops con Docker de la universidad de Helsinky

## Comandos utiles

### Ejecutar un contenedor desde una imagen

```bash
$ docker container run <nombre-imagen>
```

```bash
$ docker run <nombre-imagen>
```

### Ejecutar un contenedor desde una imagen sin retener la terminal

```bash
$ docker run -d <nombre-imagen>
```

### Detener un contenedor

```bash
$ docker stop <nombre-contenedor>
```

### Listar todas las imagenes

```bash
$ docker image ls
```

### Listar los contenedores en ejecución

```bash
$ docker container ls
```

```bash
$ docker ps
```

### Lista todos los contenedores, incluso los finalizados

```bash
$ docker container ls -a
```

### Eliminar una imagen

```bash
$ docker image rm <nombre-imagen>
```

```bash
$ docker image prune
```

### Eliminar un contenedor

```bash
$ docker container rm
```

```bash
$ docker rm
```

```bash
$ docker container prune
```

### Descargar una imagen

```bash
$ docker pull <nombre-imagen>
```
