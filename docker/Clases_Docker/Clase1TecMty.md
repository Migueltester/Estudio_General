# Docker, Redes y seguridad
Profesor Juan Velez
---

## Contenedores
### Que es un Contenedor
- Es una unidad estandarizada que contiene todos los software, dependencias, codigo y ejecutables dentro de un solo archivo
- Es un artefacto desplegable que maneja la aplicacion y sus dependencias.
- Es como un archivo zip de manera fancy
- Docker es un gestor de contenedor
- *Es un conjunto de archivos que contiene todo lo necesario para ejecutar un software, incluye librerias, codigo, y es desplegable e un ambiente controlado como docker*


## Contenedores vs maquina virtual
- Maquina virtual
  Es un Computo -> Contiene disco, ram, perifericos
  Hipervisor -> se encarga de dividir el hardware, el computo
- Contenedor
  EL Kernel -> Es la version basica del SO, para controlar el hardware
    - Pueden ejecutarse en una maquina virtual, o en un computador fisico
    - Son muchos mas ligeros y solo utilizan lo necesario del sistema operativo
    - Permiten que las aplicaciones sean portatiles
  ---

## Docker
- Es una paltaforma que permite crear, probar, e implementar aplicaciones rapidamente, permite aislar el software
- Docker no permite crear nuevos host, ya que vive dentro de uno,

## Imagenes Docker:
- Archivo que tiene metadatos que representa todos los archivos requeridos en una aplicacion contenerizada

## Arquitectura de docker
Demonio de dockerpuerto 2375 sin encriptar
Puerto 2376 para SSL


# Comandos
## Contexto 
docker context create <nombre_Del_Contexto>
---
# Infraestructura como codigo
### La infraestructura como codigo es la clave de la practica DevOps
La infraestructura como codigo es una de las metodologias devop, y un versionamiento por un modelo descriptivo para poder desplegar.
Hay una clara diferencia entre las distintas infraestructuras como codigo, y a sea terraform o cualquier otro desplegador como cloudformation, igualmente es distinto segun la nube que se utiliza, lamentablemente no es un codigo generico, si no que varia por nube.

# CloudFormation Stacks
### Son templates de stacks


## Creacion de stack a traves de S3
Se sube a un s3 y se desplega

## Actualizacion
Ya esta desplegado y te encargas de actualizarlo
## Stackset
Son todos los codigos stacks que se han realizado
## Generador de IAC 
Son plantillas de Cloudformation ya hechas

---t
# DevOps



