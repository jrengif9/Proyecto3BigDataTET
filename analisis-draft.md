# Exploración en el problema

**Problema abstracto**
	Realizar una prueba de concepto o demo sobre Data Streaming desde Twitter utilizando una de las siguientes tecnologías: Kafka, Storm, Flink o Flume.

**Contenidos**
- [Glosario](#Glosario)
	- [Prueba de Concepto](#Prueba-de-Concepto)
	- [Data Streaming](#Data-Streaming)
	- [Tecnologías](#Tecnologías)
		- [kafka](#Kafka)
		- [Storm](#Storm)
		- [Flink](#Flink)
		- [Flume](#Flume)
- [Referencias](#Referencias)
	- [Paginas](Paginas)
	- [Imágenes](Imágenes)


## Glosario:

### Prueba de Concepto

El objetivo de la prueba de concepto es valorar el concepto de producto antes de comenzar su desarrollo a nivel técnico / físico. El concepto es la idea de producto desarrollada en detalle. La ventaja inmediata es que se puede hacer fácil y rápidamente y da información para distinguir los conceptos menos valiosos. Para poder dirigir una prueba de concepto se deben tener en cuenta múltiples objetivos. [1]

### Data Streaming

Los datos de streaming son datos que se generan constantemente a partir de miles de fuentes de datos, que normalmente envían los registros de datos simultáneamente en conjuntos de tamaño pequeño (varios kilobytes). Los datos de streaming incluyen diversos tipos de datos, como archivos de registros generados por los clientes que utilizan sus aplicaciones móviles o web, compras electrónicas, actividades de los jugadores en un juego, información de redes sociales, operaciones bursátiles o servicios geoespaciales, así como telemetría de dispositivos conectados o instrumentación en centros de datos. [2]

![logSin titulo](imagenes/DataStreaming.jpg)

### Tecnologías

#### Kafka

![logSin titulo](imagenes/kafka.png)

Apache Kafka es una plataforma distribuida de Streaming utilizada para construir plataformas de procesamiento en tiempo real y permite las siguientes operaciones[3]:

-   Publicar y suscribirse a flujos de información.
-   Guardar flujos de información en un modo tolerante a fallas.
-   Procesar los flujos de información en tiempo real.

#### Storm

![logo](imagenes/storm.png)

Apache storm es un sistema computacional de código abierto distribuido en tiempo real para procesar flujos de datos. Al igual que lo que Hadoop solía hacer para el procesamiento por lotes, Apache Storm hace para flujos de datos ilimitados de una manera confiable[4].

- Capaz de procesar más de un millón de trabajos en una fracción de segundo en un nodo.
- Integrado con Hadoop para aprovechar mayores rendimientos.
- Fácil de implementar y se puede integrar con cualquier lenguaje de programación.

#### Flink

![logo](imagenes/flink.png)

Se trata de un motor de procesamiento de  **_streams_**  o  **flujos de datos**  que proporciona capacidades de distribución de datos, comunicaciones y, muy importante, tolerancia a fallos a las computaciones[5].

Cuando hablamos de computación distribuida, lo primero que se nos viene a la cabeza es el celebérrimo  Apache Hadoop,  El modelo seguido por Apache Flink fue pensado desde el principio como alternativa a MapReduce, lo que no significa que no pueda acceder y hacer uso tanto de  HDFS  o como de  YARN.

#### Flume

![logo](imagenes/flume.png)

Apache Flume es un servicio distribuido que mueve de forma fiable y eficiente grandes cantidades de datos, especialmente **logs**. Ideal para aplicaciones de analíticas en línea en **entornos Hadoop**.[6]

Flume tiene una arquitectura sencilla y flexible basada en **flujos de datos en streaming**, que permite construir flujos de múltiples por donde viajan los eventos a través de diferentes agentes hasta que alcanzan el destino final.

## Referencias

### Paginas
- [1] http://www.slmsc-project.eu/es/?page_id=2145
- [2] https://aws.amazon.com/es/streaming-data/
- [3] https://devs4j.com/2017/10/04/primeros-pasos-con-apache-kafka-en-espanol/
- [4] https://intellipaat.com/blog/what-is-apache-storm/
- [5] https://flume.apache.org/
- [6] http://www.diegocalvo.es/flume/

### Imágenes

- [1] http://muxiulin.cn/wp-content/uploads/2017/11/2f5d8fc1-c11d-4f91-aa0b-cdac4bd097fa.jpg
- [2] https://2xbbhjxc6wk3v21p62t8n4d4-wpengine.netdna-ssl.com/wp-content/uploads/2014/08/storm_2.png
- [3] https://www.paradigmadigital.com/wp-content/uploads/2017/02/flink-logo.png
- [4] https://www.tutorialspoint.com/apache_flume/images/apache_flume.jpg


<!--stackedit_data:
eyJoaXN0b3J5IjpbLTE1MTgzODkyNzIsOTQzNzk5ODU0LDE4MT
g3NzM4MjEsOTU3NDUwODY4LC0xNjQ0NTE1OTY3LDc5NjU2NzI0
MywxNDYzNTYxOTc5LC0xNDg2NjU1MzM0LDEzMDY3OTM0NTksMj
EyNTA3ODM1OSwxOTMzMjA3MTUsMjg2NDUxNTM1LC0xNjg1NTIw
OTc3LDg1MzYyNjEwNCwtNjYxMzM0Mzg4LC0xODE2NjIxOTE1LC
0yNDYwODE4Nyw5OTA3NDYwOTgsLTIwODg3NDY2MTJdfQ==
-->