# Laboratorio 3: Filtro Butterworth

Este repositorio contiene el código y documentación relacionados con el diseño e implementación de un filtro Butterworth para el filtrado de señales provenientes de un dispositivo AD8232, utilizado para monitorear señales ECG (electrocardiograma). El objetivo es diseñar un filtro pasabanda que posteriormente se convierte en un filtro pasabajo.

## Descripción del Proyecto

El AD8232 es un bloque integrado de señales para el monitoreo de ECG, diseñado para extraer, amplificar y filtrar las señales biopotenciales de baja amplitud. Para mejorar la calidad de las señales y eliminar ruido, utilizamos un filtro Butterworth de pasabanda a pasabajo, s un filtro cuya respuesta original permite el paso de señales dentro de un rango específico de frecuencias (pasabanda), pero luego se ajusta para que permita solo el paso de frecuencias más bajas, eliminando las altas frecuencias (pasa bajo). En esencia, este tipo de filtro se transforma para que su rango de paso sea más limitado y enfocado en las frecuencias más bajas.

### Filtro Butterworth

El **filtro Butterworth** es conocido por tener una respuesta en frecuencia extremadamente suave dentro de su banda de paso. Se caracteriza por:

- **Respuesta de magnitud plana en la banda de paso**: No presenta ondulaciones, lo que lo hace ideal para aplicaciones de procesamiento de señales biológicas, como ECG y EEG.
- **Atención progresiva**: En la banda de corte, la atenuación aumenta progresivamente, sin presentar transiciones abruptas.

### Parámetros del Filtro

Los parámetros del filtro se seleccionaron en base a las especificaciones del AD8232 y los requisitos de diseño del sistema:

-  -3 dB de atenuacion en 40Hz y 500Hz 
-  -40 dB de atenuacion en 4Hz y 5KHz

<img src="WhatsApp Image 2024-10-03 at 9.02.50 PM.jpeg" alt="Descripción de la imagen" width="400"/>
Figura 1. Se muestra como se ve el filtro pasabanda con sus respectivos datos.

