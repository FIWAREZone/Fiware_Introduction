# Introducción

Este curso tiene el objetivo de ayudar a comprender las operaciones básicas y servir de punto inicial para empezar a trabajar con FIWARE. En este curso se tratará el modelado de entidades y los atributos de esta, así como las operaciones básicas para crear, editar y borrar las entidades, además de hacer búsqueda de estas en función de los valores de sus atributos. En este curso se empleará la versión 2 del protocolo NGSI.

## Conocimientos previos

Para la realización del curso es conveniente disponer de conocimientos básicos de APIs REST / HTTP y conocimientos básicos de redes.

## FIWARE

El objetivo de este taller es aprender a usar de una forma básica la API NGSI de FIWARE para el envío de datos y su posterior recuperación del context broker, así como otra serie de operaciones.

# Configuración del entorno

En esta sección repasaremos como instalar y configurar los programas necesarios para desarrollar el curso. Será necesario disponer instalada correctamente la utilidad Postman así como la colección de peticiones de este repositorio y el entorno correctamente configurado

## Instalación de Postman

Para hacer pruebas con la API de FIWARE será necesario disponer de una herramienta que permita hacer peticiones HTTP e interactuar con esta. En este caso, nosotros recomendamos la herramienta Postman, que permite gestionar las colecciones de peticiones, por lo que será muy sencillo realizar las operaciones necesarias.

[https://www.getpostman.com](https://www.getpostman.com)

Una vez instalada la aplicación, es necesario importar la colección de peticiones así como el entorno que tiene las variables empleadas en la colección. Ambos ficheros están alojados en este mismo repositorio y se pueden descargar clonándolo.

## Variables de entorno

Una vez hayamos importado tanto la colección de peticiones como el entorno (los dos ficheros descargados en el punto anterior) 

Las variables de entorno contienen parámetros que se aplican a todas las colecciones pero, que para facilitar cambiarlas todas a las vez, se han hecho variables de entorno, como por ejemplo la URL del servidor. Es necesario modificar las variables de entorno con los parámetros correspondientes:

| Parametro         |descripción   												|
| :-----------------|:--------------											|
| user              | Usuario con permisos de acceso							|
| password          | Contraseña del Usuario 									|
| service   		| Servicio del contex broker (Header Fiware-Service) 		|
| subservice      	| Subservicio del context broker (Header Fiware-ServicePath) |
| token 			| Token de autenticación de usuario dinámico 				|
| host 				| URL del servidor, es decir, del Orion Context Broker 		|



