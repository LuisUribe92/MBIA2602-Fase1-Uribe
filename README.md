# MBIA2602-Fase1-Uribe
Chatbot creado como un asistente de diagnóstico rápido, diseñado específicamente para reducir el tiempo muerto (downtime) de producción y bajar el MTTR relacionado a máquinas de aplicación de conformal.

# Asistente Inteligente de Mantenimiento – Para máquinas de aplicación de conformal 

Ese es un chatbot interactivo basado en Reglas y Procesamiento de Lenguaje Natural (NLP) utilizando la librería `NLTK` en Python. Su objetivo principal es guiar a los técnicos de mantenimiento y operadores en el diagnóstico acelerado de fallas de proceso (goteo, obstrucciones, burbujas, presión) en máquinas de conformal coating **Nordson Asymtek SL-940**, ayudando a reducir el MTTR (Tiempo Promedio de Reparación).
Desarrollado por: **Ing. Luis Uribe**  
Rol: **Ingeniero de Procesos Sr**

##  Requisitos e Instalación

Este proyecto requiere **Python 3.10 o superior** y la librería `nltk`.
*Nota: Si utilizas **Google Colab**, la instalación se realiza automáticamente en la primera celda mediante el comando `%pip -q install nltk` incluido en el código fuente. *

---
##  Ejemplos de Uso (Conversaciones)

Al ejecutar el chatbot en la terminal, puedes interactuar ingresando problemas comunes de la máquina. El sistema identificará la intención y te proveerá la solución:

```text
Tu: La boquilla está goteando material
Intencion: falla_goteo
Bot: [Causa Raíz - Goteo]: 1. Aire atrapado en la cámara del fluido (requiere purga). 2. Presión de aire de asistencia insuficiente. 3. Desgaste en la aguja o asiento de la valvula (SC-400/SC-280).

Tu: software y presion
Intencion: ambigua
Bot: Por favor, consulta un solo síntoma a la vez para evitar confusiones de diagnóstico.

Tu: salir
Intencion: salir
Bot: Sesion finalizada.
```
