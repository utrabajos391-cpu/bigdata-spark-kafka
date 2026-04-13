# Proyecto Big Data - Spark Streaming y Kafka

## Descripción
Este proyecto implementa un sistema de procesamiento de datos en tiempo real utilizando Apache Kafka y Apache Spark Streaming.

## Tecnologías utilizadas
- Apache Kafka
- Apache Spark
- Python

## Funcionamiento

1. Se crea un productor que genera datos simulados de sensores.
2. Los datos se envían a un topic de Kafka llamado `sensor_data`.
3. Spark Streaming consume los datos en tiempo real.
4. Se procesan los datos calculando promedios de temperatura y humedad por sensor.

## Archivos

- kafka_producer.py → Genera y envía datos
- spark_streaming_consumer.py → Procesa datos en tiempo real

## Ejecución

### Ejecutar productor:
python3 kafka_producer.py

### Ejecutar consumidor:
spark-submit --packages org.apache.spark:spark-sql-kafka-0-10_2.12:3.5.3 spark_streaming_consumer.py

## Autor
Rodolfo Suarez Hernandez
