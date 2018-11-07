# Informe de Análisis

Análisis mas detallado acerca del proyecto a trabajar, ademas abordando mas profundamente los temas de arquitecturas de datos y como estos interactuan con el software a utilizar.

**Contenidos:**

- [Problemáticas](#Problemáticas)
	- [Problemas abstracto](#Problema-abstracto)
	- [Problema especifico](#Problema-especifico)
- [Aquitectura preliminar](#arquitectura-preliminar-de-datos-ciclo-de-vida-almacenamiento-procesamiento)
- [fuentes y naturaleza de los datos](#fuentes-y-naturaleza-de-los-datos--tecnologías-a-utilizar)
- [sistema de ingesta de datos](#sistema-de-ingesta-de-datos--tecnologías-a-utilizar)
- [almacenamiento de los datos](#almacenamiento-de-los-datos--tecnologías-a-utilizar)
- [análisis de datos](#análisis-de-datos--tecnologías-a-utilizar)






## Problemáticas

### Problema abstracto

Realizar una prueba de concepto o demo sobre Data Streaming desde Twitter utilizando una de las siguientes tecnologías: Kafka, Storm, Flink o Flume.

### Problema especifico

Actualmente las **redes sociales** se ven abatidas por **reacciones de los usurarios** a ciertos eventos que se presentan en sus comunidades, ciudades países y hasta a nivel mundial. Dichos eventos mediáticos son de gran importancia en redes sociales como **twitter**  donde se almacenan estos datos que esperan ser analizados y estudiados por personas interesadas en ellos.


![Ver Noticia](imagenes/Noticia.PNG)
[Ver Noticia](https://elpais.com/internacional/2018/09/06/actualidad/1536217018_424450.html)

Uno de esos eventos mediáticos ha sido la aprobación o desaprobación en ciertos paíises sobre políiticas relacionadas con la comunidad LGBT en temas como:

- Igualdad de derechos.
-  Adopción de parejas del mismo sexo.
- Matrimonio igualitario.

Analizar estos temas ayudaría tomar mejores decisiones a ciertos sectores de la sociedad y hasta llegar a generar políticas publicas que combatan cierta clase de acoso hacia esta comunidad.

**Objetivo:** Analizar publicaciones realizadas en la red social tomar mejorwitter sobre comentarios que contengan palabras claves relacionadas con politicas hacia la comunidad LGBTI y determinar que porcentaje de dichos comentarios tienen una posición positiva, neutra o negativa.


## Arquitectura preliminar de datos (ciclo de vida, almacenamiento, procesamiento)

 **Ciclo de Vida:**  El ciclo de vida de los datos comienza en los Tweets que producen los usurios de Twitter, aquellos tweets deben estar relacionados con unas palabras a las que llamaremos  **keywords**, que para nuestro caso son "Coca-cola" y "Pepsi". Twitter entonces proveera una interfaz por medio de una API ([Apps Twitter](https://apps.twitter.com/)), dicha API sera accedida por un agente que tomara los datos bajo tecnicas de DataStreaming y lo almacenara en alguna tecnologia de Storage (Para el caso HDFS).
 

 **Almacenamiento:**  Dado que es un proceso constante e inserción de datos, es fundamental tener un sistema de almacenamiento escalable que garantice el acceso a los datos, y que ojalá sea de una manera sencilla. Inicialmente los datos son extraidos con un formato  [JSON](https://es.wikipedia.org/wiki/JSON)  del cual pueden extraerse atributos fundamentales para el análisis.

## Fuentes y naturaleza de los datos + tecnologías a utilizar.

## Sistema de ingesta de datos + tecnologías a utilizar.

### Apache Flume

Flume es un servicio distribuido, confiable y disponible para recopilar, agregar y mover de manera eficiente grandes cantidades de datos de registro. Tiene una arquitectura simple y flexible basada en flujos de datos de transmisión. Es robusto y tolerante a fallas con mecanismos de confiabilidad sintonizables y muchos mecanismos de recuperación y recuperación de fallas. Utiliza un modelo de datos extensible simple que permite la aplicación analítica en línea.

## Almacenamiento de los datos + tecnologías a utilizar.

### HDFS

### Apache Hive

## Análisis de datos + tecnologías a utilizar.

## Referencias

- [1] https://flume.apache.org/
<!--stackedit_data:
eyJoaXN0b3J5IjpbLTE0MTU2MTMwLC0zMTkzMDY4MTcsMTA4MT
IzNjA3NiwtMTI2ODIyODE4NCwxNDc0NzUyMDk4LDE5NjAzMDYx
NTEsMzE0NDgzMzMxLC0xMzE1OTc5MTQzLDE4OTEyMTk3NzIsMz
Q2NTExOTk2LDE0MzA5NTgyNjAsLTIxMzc4MTkwMTksLTQ4NjM5
ODQ2MiwtMTIwNTM3ODIxLC0xODMwOTgxNTYwLC0yMDg4NzQ2Nj
EyLDk4MzY0NjUwNl19
-->