# Taller De Redes IRC

Dockerfiles para montar un cliente y servidor IRC con la finalidad de generar y analizar el trafico IRC generado por los estos.
Autores: Matías Ringeling - David Pazán

## Clonar repositorio
En primer lugar se ha de clonar el repositorio, y se procede a instalar el servidor y cliente
```
https://gitlab.com/tareas-taller-de-redes-y-servicios-2021-1/2021-2/grupo_1.git
```

## Instalar servidor

```
cd Servidor/
sudo docker build . -t servidor
```

## Instalar cliente

```
cd Cliente/
sudo docker build . -t cliente

```

## Instalar polymorph

```
cd Polymorph/
sudo docker build . -t polymorph

```
# Uso

A continuación los comandos para ejecutar los docker.

```
sudo docker run -it -p 6667:6667 --name servidor_irc servidor
```

```
sudo docker run -it --name cliente_irc cliente

```

```
sudo docker run --privileged -it --name Polymorph polymorph

```

# Video demostracion
[![Video Demostración](https://i.imgur.com/OBBkrFU.png)](https://youtu.be/LPEkf3mqnRoY)

# Video demostración modificación de tráfico
[![Video demostración modificación de tráfico](https://i.imgur.com/KVpjjDR.png)](https://youtu.be/x5IGxQmZp2k)

