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
 
 ![Sintitulo](https://picasaweb.google.com/112351682247760038310/6621239582374091009#6621239579488911762 "Sin titulo")

 **Almacenamiento:**  Dado que es un proceso constante e inserción de datos, es fundamental tener un sistema de almacenamiento escalable que garantice el acceso a los datos, y que ojalá sea de una manera sencilla. Inicialmente los datos son extraidos con un formato  [JSON](https://es.wikipedia.org/wiki/JSON)  del cual pueden extraerse atributos fundamentales para el análisis.

## Fuentes y naturaleza de los datos + tecnologías a utilizar.

## Sistema de ingesta de datos + tecnologías a utilizar.

### Apache Flume

Flume es un servicio distribuido, confiable y disponible para recopilar, agregar y mover de manera eficiente grandes cantidades de datos de registro. Tiene una arquitectura simple y flexible basada en flujos de datos de transmisión. Es robusto y tolerante a fallas con mecanismos de confiabilidad sintonizables y muchos mecanismos de recuperación y recuperación de fallas. Utiliza un modelo de datos extensible simple que permite la aplicación analítica en línea.

## Almacenamiento de los datos + tecnologías a utilizar.

### HDFS

El Sistema de archivos distribuidos de Hadoop (HDFS) es un sistema de archivos distribuidos diseñado para ejecutarse en hardware básico. Tiene muchas similitudes con los sistemas de archivos distribuidos existentes. Sin embargo, las diferencias con otros sistemas de archivos distribuidos son significativas. HDFS es altamente tolerante a fallos y está diseñado para implementarse en hardware de bajo costo. HDFS proporciona acceso de alto rendimiento a los datos de la aplicación y es adecuado para aplicaciones que tienen grandes conjuntos de datos. HDFS relaja algunos requisitos POSIX para permitir el acceso de transmisión a los datos del sistema de archivos. HDFS se creó originalmente como infraestructura para el proyecto del motor de búsqueda web Apache Nutch. HDFS es ahora un subproyecto Apache Hadoop.

### Apache Hive

Apache Hive es un proyecto de código abierto ejecutado por voluntarios en Apache Software Foundation. Anteriormente, era un subproyecto de **Apache® Hadoop®**, pero ahora se ha graduado para convertirse en un proyecto de alto nivel. Lo alentamos a que conozca el proyecto y aporte su experiencia.

## Análisis de datos + tecnologías a utilizar.

## Referencias

- [1] https://flume.apache.org/
- [2] https://hadoop.apache.org/docs/r1.2.1/hdfs_design.html
<!--stackedit_data:
eyJoaXN0b3J5IjpbMTk3Mjg1NjIzMiwtMTUwNjAyNjQ0MCwtMT
QxNTYxMzAsLTMxOTMwNjgxNywxMDgxMjM2MDc2LC0xMjY4MjI4
MTg0LDE0NzQ3NTIwOTgsMTk2MDMwNjE1MSwzMTQ0ODMzMzEsLT
EzMTU5NzkxNDMsMTg5MTIxOTc3MiwzNDY1MTE5OTYsMTQzMDk1
ODI2MCwtMjEzNzgxOTAxOSwtNDg2Mzk4NDYyLC0xMjA1Mzc4Mj
EsLTE4MzA5ODE1NjAsLTIwODg3NDY2MTIsOTgzNjQ2NTA2XX0=

-->