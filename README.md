#🧾 Sistema de Administración de Tareas
##💼 Trabajo Práctico Integrador – Fundamentos de Spring Boot

Carrera: Ingeniería en Sistemas de Información
Materia: Desarrollo de Software

##🎯 Objetivo Principal

El propósito de este proyecto es aplicar los fundamentos esenciales de Spring Boot mediante la creación de una aplicación profesional para la gestión de tareas (To-Do List).

Durante el desarrollo se implementan los siguientes conceptos clave:

💉 Inyección de dependencias

🧱 Estereotipos: @Service, @Repository, @Component

⚙️ Configuración externa mediante application.properties

🌐 Profiles (dev y prod) para manejar distintos entornos de ejecución

##🧠 Descripción del Proyecto

El sistema permite administrar tareas de manera simple, estructurada y adaptable a diferentes entornos.

###Funcionalidades principales:

📋 Listar tareas existentes

➕ Agregar nuevas tareas

✅ Marcar tareas como completadas

📊 Consultar estadísticas de progreso

⚙️ Adaptar comportamiento según el entorno (desarrollo o producción)

Cada entorno ajusta sus mensajes, límites y niveles de log según el Profile configurado.

##🧩 Estructura del Proyecto
com.utn.tareas
├── model
│   ├── Tarea.java
│   └── Prioridad.java
├── repository
│   └── TareaRepository.java
├── service
│   ├── TareaService.java
│   ├── MensajeService.java
│   ├── MensajeDevService.java
│   └── MensajeProdService.java
└── TareasApplication.java

##⚙️ Tecnologías Utilizadas
Tecnología	Versión	Descripción
☕ Java	17+	Lenguaje principal
🧩 Spring Boot	3.x	Framework para el desarrollo backend
⚙️ Maven	-	Sistema de gestión de dependencias
✨ Lombok	-	Reducción del código boilerplate
🔁 Spring Boot DevTools	-	Recarga automática en desarrollo

##🚀 Ejecución del Proyecto
Para ejecutar el proyecto con Maven, usar el siguiente comando:

mvn spring-boot:run

1️⃣ Clonar el repositorio
git clone https://github.com/usuario/tareas-springboot.git
cd tareas-springboot

##🔧 Configuración de Perfiles

El comportamiento de la aplicación se determina según el profile activo definido en el archivo:

src/main/resources/application.properties

spring.profiles.active=dev  # o prod

##🔹 Entorno de Desarrollo (DEV)

Archivo: application-dev.properties

app.max-tareas=10
app.mostrar-estadisticas=true
logging.level.com.utn.tareas=DEBUG


###Características:

✅ Mensajes detallados

📊 Estadísticas activadas

💻 Límite reducido de tareas

##🔸 Entorno de Producción (PROD)

Archivo: application-prod.properties

app.max-tareas=1000
app.mostrar-estadisticas=false
logging.level.com.utn.tareas=ERROR


###Características:

🚀 Mensajes simplificados

📉 Estadísticas deshabilitadas

📈 Mayor cantidad máxima de tareas

🖼️ Evidencias en Consola
🧱 Perfil de Producción

💻 Perfil de Desarrollo

##🧾 Conclusiones

El desarrollo de este proyecto me permitió comprender en profundidad el ecosistema de Spring Boot y su relevancia en el desarrollo de aplicaciones modernas con Java.

La inyección de dependencias demostró ser clave para lograr un código modular, desacoplado y más fácil de mantener.

Por otro lado, la práctica con profiles y configuraciones externas permitió observar cómo un mismo proyecto puede adaptarse fácilmente a diferentes entornos (desarrollo y producción) sin alterar su código fuente.

Finalmente, el uso de anotaciones como @Service, @Repository y @Profile reforzó la importancia de las buenas prácticas, la organización del código y la claridad en la arquitectura del proyecto.

En conjunto, esta experiencia me brindó una visión más profesional y sólida sobre el desarrollo con Spring Boot.

##👤 Autor

Nicolas Andres Moreno Coll 
Legajo 50989
