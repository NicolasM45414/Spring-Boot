<h1 align="center">📝 Sistema de Administración de Tareas</h1> <p align="center"> <b>Trabajo Práctico Integrador – Fundamentos de Spring Boot</b><br> <i>Ingeniería en Sistemas de Información – Desarrollo de Software</i> </p>
🎯 Propósito del Proyecto

El objetivo principal es poner en práctica los conocimientos esenciales de Spring Boot, desarrollando una aplicación profesional para la gestión de tareas (To-Do List), implementando los siguientes conceptos:

Inyección de dependencias

Uso de estereotipos (@Service, @Repository, @Component)

Configuración mediante application.properties

Utilización de perfiles (dev y prod) para distintos entornos de ejecución

🧠 Descripción General

El proyecto se basa en un sistema que permite administrar tareas de manera sencilla y eficiente. Entre sus funcionalidades se incluyen:

📋 Visualizar el listado de tareas existentes

➕ Registrar nuevas tareas

✅ Cambiar el estado de una tarea a completada

📊 Consultar estadísticas de progreso

⚙️ Adaptar la configuración según el entorno de ejecución (desarrollo o producción)

Cada perfil modifica ciertos parámetros, como mensajes, límites o niveles de log, en función del Profile seleccionado.

🧩 Organización del Proyecto
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

⚙️ Tecnologías Empleadas
Tecnología	Versión	Descripción
☕ Java	17+	Lenguaje principal del proyecto
🧩 Spring Boot	3.x	Framework base para el backend
⚙️ Maven	-	Herramienta para la gestión de dependencias
✨ Lombok	-	Simplifica y reduce código repetitivo
🔁 Spring Boot DevTools	-	Permite recarga automática en tiempo de desarrollo
🚀 Instrucciones para la Ejecución

Para ejecutar el proyecto mediante Maven, usar el siguiente comando:

mvn spring-boot:run

1️⃣ Clonar el repositorio
git clone https://github.com/usuario/tareas-springboot.git
cd tareas-springboot

🔧 Configuración de Perfiles

El comportamiento de la aplicación se define según el profile activo, especificado en el archivo:

src/main/resources/application.properties

spring.profiles.active=dev  # o prod

🔹 Entorno de Desarrollo (DEV)

Archivo: application-dev.properties

app.max-tareas=10
app.mostrar-estadisticas=true
logging.level.com.utn.tareas=DEBUG


✅ Mensajes detallados

📊 Estadísticas activadas

💻 Límite reducido de tareas

🔸 Entorno de Producción (PROD)

Archivo: application-prod.properties

app.max-tareas=1000
app.mostrar-estadisticas=false
logging.level.com.utn.tareas=ERROR


🚀 Mensajes simplificados

📉 Estadísticas deshabilitadas

📈 Mayor capacidad de tareas

📸 Ejemplos en Consola (Profiles)

Perfil de Producción:
<img width="654" height="555" alt="produccion" src="https://github.com/user-attachments/assets/448e7180-7a39-459a-b1a4-0e403bf672a3" />

Perfil de Desarrollo:
<img width="646" height="621" alt="desarrollo" src="https://github.com/user-attachments/assets/c3ac1d29-6163-4791-8986-702ed5a74d79" />

🧾 Conclusión

Durante el desarrollo de este trabajo integrador pude profundizar en el funcionamiento del ecosistema de Spring Boot, comprendiendo por qué se ha convertido en una de las herramientas más potentes para el desarrollo moderno con Java.

La inyección de dependencias resultó clave para entender la importancia de un código desacoplado y modular, mejorando la mantenibilidad y escalabilidad del sistema.

Asimismo, la configuración por perfiles me permitió experimentar cómo un mismo proyecto puede adaptarse fácilmente a distintos entornos (desarrollo y producción) sin alterar su código base.

Finalmente, reforcé el uso de anotaciones como @Service, @Repository y @Profile, que contribuyen a una estructura más clara y ordenada. Este trabajo me permitió adquirir una visión más profesional sobre las buenas prácticas y arquitectura de aplicaciones con Spring Boot.

👤 Autor

Nicolas Andres Moreno Coll – Legajo 50989
