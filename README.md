<img src="images/neteclogo.png" alt="logo" width="300"/>

# Administración de Confluent Apache Kafka

## Plataforma de laboratorios

Te damos la bienvenida a la **plataforma de laboratorios** del curso **Administración de Confluent Apache Kafka**. Aquí podrás explorar diferentes tecnologías a través de prácticas guiadas. ¡Desarrolla tus habilidades y lleva tus conocimientos al siguiente nivel!

El curso se apoya en un caso narrativo — la operación de **NovaTech Logistics** — y construye, capítulo a capítulo, un clúster Kafka 4.2 sobre Confluent Platform 8.2.0 en modo KRaft: desde encender el primer broker hasta asegurarlo con TLS, SASL y ACLs.

**Stack:** Apache Kafka 4.2 · Confluent Platform 8.2.0 · KRaft (sin ZooKeeper) · Java 21 · Docker Compose

## Lista de laboratorios

Cada uno de estos laboratorios está diseñado para ofrecerte una experiencia práctica. Haz clic en los enlaces para comenzar.

### [Práctica 0. Validación del entorno](Capitulo_1/README.md)

  - **Descripción**: Fundamentos de arquitectura y ecosistema, y verificación de que tu máquina está lista para correr los 14 laboratorios.
  - ⏱️ **Duración estimada**: 30 min.

### [Práctica 1. Inicialización de un clúster KRaft](Capitulo_2/lab-01-inicializacion-kraft/README.md)

  - **Descripción**: Genera el cluster-id, formatea el storage y levanta tu primer broker KRaft pieza por pieza.
  - ⏱️ **Duración estimada**: 60 min.

### [Práctica 2. Validación de quórum y resiliencia](Capitulo_2/lab-02-validacion-quorum-resiliencia/README.md)

  - **Descripción**: Completa el quórum de tres controladores y comprueba qué sobrevive cuando cae un nodo.
  - ⏱️ **Duración estimada**: 60 min.

### [Práctica 3. Configuración de brokers](Capitulo_3/lab-03-configuracion-brokers/README.md)

  - **Descripción**: Anatomía del archivo de configuración: qué parámetro toca qué, y cómo verificarlo dentro del contenedor.
  - ⏱️ **Duración estimada**: 60 min.

### [Práctica 4. Clúster multi-broker y advertised.listeners](Capitulo_3/lab-04-multibroker-advertised-listeners/README.md)

  - **Descripción**: El parámetro que más clústeres rompe: separación de listeners y conectividad desde fuera del contenedor.
  - ⏱️ **Duración estimada**: 60 min.

### [Práctica 5. Operación de tópicos](Capitulo_3/lab-05-operacion-topicos/README.md)

  - **Descripción**: Crear, describir, alterar y dimensionar tópicos como lo haría un DBA sobre sus tablas.
  - ⏱️ **Duración estimada**: 60 min.

### [Práctica 6. Producción y consumo desde CLI](Capitulo_3/lab-06-produccion-consumo-cli/README.md)

  - **Descripción**: Productores y consumidores desde la línea de comandos, grupos de consumo y lectura de offsets.
  - ⏱️ **Duración estimada**: 60 min.

### [Práctica 7. Pruebas de rendimiento](Capitulo_3/lab-07-pruebas-rendimiento/README.md)

  - **Descripción**: Mide throughput y latencia con las herramientas nativas, y observa el efecto de I/O, red, RAM y CPU.
  - ⏱️ **Duración estimada**: 90 min.

### [Práctica 8. Cambio de configuración de brokers en caliente](Capitulo_3/lab-08-brokers-en-caliente/README.md)

  - **Descripción**: Reconfiguración dinámica sin reiniciar el clúster, y adición de un cuarto broker en operación.
  - ⏱️ **Duración estimada**: 60 min.

### [Práctica 9. Clientes Java y Spring](Capitulo_4/lab-09-clientes-java-spring/README.md)

  - **Descripción**: Productor y consumidor en Java puro y su equivalente en Spring Boot 4.1 con spring-kafka.
  - ⏱️ **Duración estimada**: 60 min.

### [Práctica 10. REST Proxy](Capitulo_4/lab-10-rest-proxy-kafbat-ui/README.md)

  - **Descripción**: Produce y consume por HTTP sin cliente Kafka, y explora el clúster visualmente con Kafbat UI.
  - ⏱️ **Duración estimada**: 60 min.

### [Práctica 11. Schema Registry](Capitulo_4/lab-11-schema-registry/README.md)

  - **Descripción**: Contratos de datos con Avro, evolución de esquemas y modos de compatibilidad.
  - ⏱️ **Duración estimada**: 60 min.

### [Práctica 12. ksqlDB](Capitulo_5/lab-12-ksqldb/README.md)

  - **Descripción**: Procesamiento de streams con SQL: STREAMS, TABLES y consultas continuas sobre los tópicos.
  - ⏱️ **Duración estimada**: 60 min.

### [Práctica 13. Kafka Connect](Capitulo_5/lab-13-kafka-connect/README.md)

  - **Descripción**: Integra Kafka con PostgreSQL mediante connectors source y sink, sin escribir código.
  - ⏱️ **Duración estimada**: 60 min.

### [Práctica 14. Capstone — Resiliencia y seguridad](Capitulo_5/lab-14-capstone-resiliencia-seguridad/README.md)

  - **Descripción**: Clúster asegurado con TLS, SASL y ACLs, sometido a una prueba de failover sin pérdida de mensajes.
  - ⏱️ **Duración estimada**: 120 min.

---

## Validación del entorno

El curso incluye un **botón único de validación** que audita tu plataforma y, opcionalmente, ejecuta el harness completo de los 14 laboratorios sobre Docker real:

```bash
./validar-todo.sh --solo-preflight   # verificación rápida de la plataforma
./validar-todo.sh                    # validación funcional completa (Docker real)
```

Si algo falla, `scripts/diagnostico/validar-ambiente.sh` revisa lab por lab los prerrequisitos concretos (puertos, imágenes, RAM asignada a Docker).

---

## 📬 **Contacto y más información**

Si tienes alguna pregunta o necesitas más detalles, no dudes en [contactarnos](mailto:soporte@netec.com). También puedes encontrar más recursos en nuestra [página](https://netec.com).

---

¡Gracias por visitar nuestra plataforma! No olvides revisar todos los laboratorios y comenzar tu viaje de aprendizaje hoy mismo.
