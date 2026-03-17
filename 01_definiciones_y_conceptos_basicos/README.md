# Definiciones y conceptos básicos

## DevOps

_DevOps es una metodología de desarrollo destinada a cerrar la brecha entre
`Desarrollo` y `Operaciones`, haciendo hincapié en la comunicación y la
colaboración, la integración continúa, el aseguramiento de la calidad y la
entrega con despliegue automatizado utilizando un conjunto de prácticas de
desarrollo._

## Docker

_Docker es un conjunto de productos de plataforma como servicio
(Platform as a service - PaaS) que utilizan virtualización a nivel del sistema
operativo para distribuir software en paquetes llamados `contenedores`._

1. Docker es un conjunto de herramientas para distribuir software en
   contenedores.
2. Contenedores son paquetes de software.

## Imagen

_Una imagen de Docker es un archivo. Una imagen nunca cambía. La creación de una
nueva imagen sucede comenzando con una imagen base y añadiendole nuevas capas._

`Dockerfile` &rarr; `Imagen` &rarr; `Contenedor`

## Contenedor

_Un contenedor contiene una aplicación y todo lo necesario para su ejecución.
Puedes comenzarlo, detenerlo o interactuar con el. Son entornos aislados en la
**máquina host** con la habilidad de interactuar con otros contenedores y la
propia **máquina host** por métodos definidos (TCP/UDP)._
