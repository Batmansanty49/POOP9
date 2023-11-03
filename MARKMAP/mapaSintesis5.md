# Diagramas de secuencia

## Etapas de la creación
### Etapa 1
#### Los orígenes del enfoque orientado a objetos el cual ganó popularidad en la década de 1980.
### Etapa 2
#### En el uso de los diagramas de colaboración, antes de los diagramas de secuencia.
### Etapa 3
#### El desarrollo de UML.
### Etapa 4
#### La adopción generalizada de los diagramas de secuencia.
### Etapa 5
#### La evolución continua de los diagramas de secuencia y su uso en la ingeniería de software.
## ¿Qué son?
### Son diseños geométricos que se representan gráficamente como: 
#### ideas, procesos, soluciones, mecanismos o fenómenos.

## Ventajas
### Son útiles para comprender y comunicar cómo interactúan los diferentes elementos de un sistema.
#### Los hace valiosos en el diseño, análisis y documentación de sistemas de software.
#### Son parte importante de la notación UML.

### Ventajas a comparación con otros diagramas
#### Representación de interacciones temporales:
##### son ideales para representar las interacciones entre objetos a lo largo del tiempo.
#### Enfoque en el comportamiento:
##### se centran en el comportamiento dinámico.
#### Identificación de problemas de diseño:
##### pueden ayudar a identificar problemas de diseño o de comunicación entre objetos
#### Documentación y comunicación efectiva:
##### una herramienta efectiva para documentar y comunicar el diseño de software a las partes interesadas
#### Soporte para pruebas y depuración:
##### proporcionan una representación clara de las interacciones esperadas entre objetos.
#### Modelado de casos de uso:
##### ilustran cómo se llevarán a cabo las interacciones entre actores y objetos en un escenario específico.
#### Compatibilidad con otras vistas UML:
##### se puede utilizar junto con otros tipos de diagramas  UML:
###### diagramas de clases
###### diagramas de actividad
###### diagramas de estado

## Desventajas
### Complejidad visual:
#### pueden volverse complejos y difíciles de entender cuando el sistema es grande con numerosos objetos.

### Limitaciones en la representación de estructura:
#### no están diseñados principalmente para representar la estructura del sistema.

### Foco en la secuencia temporal:
#### se centran en mostrar la secuencia temporal de interacciones entre objetos.

### No adecuados para todos los tipos de sistemas:
#### pueden ser menos útiles para sistemas que no siguen un enfoque orientado a objetos.

### Limitaciones en la representación de datos:
#### pero no son ideales para mostrar cómo los datos fluyen a través del sistema

### No son adecuados para todos los aspectos del ciclo de vida del software:
#### pueden ser menos útiles en otras etapas del ciclo de vida del software.

## Características
### Representación Visual:
#### permiten representar la secuencia de interacciones entre objetos en un sistema.

### Objetos y Roles:
#### los objetos se representan como rectángulos verticales.
#### Se pueden asignar roles a los objetos para especificar sus funciones.

### Líneas de Vida:
#### son líneas verticales que representan la existencia temporal de un objeto en el diagrama.

### Mensajes:
#### son flechas que conectan las líneas de vida de los objetos y representan las interacciones entre ellos.
#### los mensajes pueden ser:
##### síncronos (bloqueantes)
##### asíncronos (no bloqueantes)

### Activación y Desactivación:  
#### muestran la activación y desactivación de objetos en el tiempo.

### Fragmentos de Interacción:
#### permiten modelar escenarios de interacción alternativos o paralelos.

### Condiciones y Bucles:
#### representan la lógica de control dentro de una interacción.

### Tiempo y Duración:
#### Es posible especificar la duración de una interacción o el tiempo que lleva que un objeto responda a un mensaje.

### Desarrollo Iterativo:
#### se utilizan en las etapas de análisis y diseño de un proyecto de desarrollo de software.

### Documentación y Comunicación: 
#### forma efectiva de documentar, comunicar la arquitectura y el comportamiento del sistema.


## Estructuras
### Participantes:
#### Actores:
##### representan entidades externas al sistema que interactúan con él
###### se dibujan generalmente en la parte superior del diagrama.
#### Objetos: 
##### son las entidades internas que realizan las operaciones dentro del sistema
###### los objetos se ubican en la parte inferior. 

### Líneas de Vida (Lifelines):
#### Cada objeto o actor tiene una línea de vida asociada que representa su existencia en el tiempo.

### Mensajes:
#### Síncrono:
##### Representa una llamada de método que bloquea al remitente hasta que el receptor termine de procesar el mensaje.
#### Asíncrono:
##### Indica una llamada de método que no bloquea al remitente, permitiendo que continúe su ejecución sin esperar una respuesta inmediata del receptor.

### Fragmentos de Activación:
#### Condiciones (guardas):
##### En algunos casos es necesario especificar las condiciones para mostrar en qué condiciones se ejecutan ciertas interacciones.
#### Iteraciones y Alternativas:
##### se utilizan para modelar comportamientos repetitivos o ramificaciones en el flujo de ejecución del sistema.
#### Mensajes de Retorno:
##### muestran la respuesta del receptor al remitente.
#### Fragmentos de Opción:
##### se utilizan para mostrar múltiples caminos alternativos en un diagrama de secuencia. 
#### Fragmentos de Bucle:
##### representan repeticiones en un diagrama de secuencia y se utilizan para modelar ciclos o iteraciones en la interacción entre objetos.
#### Fragmentos de Alternativa:
##### permiten modelar situaciones en las que se debe tomar una decisión y seguir diferentes caminos en función de una condición.


## Utilidad
### Representación Del Flujo de Interacción:
#### capturan la dinámica de un sistema.

### Diseño De Sistemas:
#### permite una planificación más efectiva y la identificación temprana de posibles problemas del diseño.

### Identificación De Problemas De Diseño:
#### permite realizar ajustes en la arquitectura del sistema para mejorar su eficiencia y rendimiento.

### Verificación De Requisitos:
#### asegura que las interacciones se produzcan de acuerdo con las especializaciones.

### Pruebas:
#### ayuda a garantizar que todas las interacciones se prueben adecuadamente.

### Optimización De Rendimiento:
#### implica reducir la carga de comunicación entre objetos, optimizar la distribución de tareas y garantizar una ejecución eficiente.


## Diferencia entre este y otros diagramas UML
### Enfoque en la interacción temporal:
#### permite comprender el flujo de control y la sincronización en un escenario específico de ejecución.

### Relación con otros diagramas:
#### se centran en la estructura de los objetos y las relaciones entre ellos.

### Enfoque en la ejecución:
#### es útil para comprender la lógica de ejecución y la comunicación entre objetos en una situación dada.



## Todos los tipos de mensajes
### de invocacción:
#### representa una llamada a un método o función de un objeto.

### de respuesta:
#### para representar la respuesta de un objeto a una llamada de método.

### de creación:
#### se utiliza para representar la creación de un nuevo objeto dentro del sistema.

### de destrucción:
#### representa la eliminación de un objeto del sistema.

### de llamada asíncrona
#### representar una llamada a un método en la que el objeto que envía

### de sincronización:
#### representa la sincronización de múltiples objetos en un punto específico del diagrama de secuencia.

### de temporizador:
#### representar eventos temporizados que generan una acción en el sistema.