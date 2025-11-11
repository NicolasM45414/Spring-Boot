<h1 align="center">🧾 Sistema de Administración de Tareas</h1>

<p align="center">
  <b>💼 Trabajo Práctico Integrador – Fundamentos de Spring Boot</b><br>
  <i>Carrera: Ingeniería en Sistemas de Información-Materia: Desarrollo de Software/i>
</p>

---

## 🎯 Objetivo

El propósito de este proyecto es aplicar los fundamentos esenciales de Spring Boot mediante la creación de una aplicación profesional para la gestión de tareas (To-Do List).

Durante el desarrollo se implementan los siguientes conceptos clave:

💉 Inyección de dependencias

🧱 Estereotipos: @Service, @Repository, @Component

⚙️ Configuración externa mediante application.properties

🌐 Profiles (dev y prod) para manejar distintos entornos de ejecución

---

## 🧠 Descripción del Proyecto

El sistema permite administrar tareas de manera simple, estructurada y adaptable a diferentes entornos.

###Funcionalidades principales:

📋 Listar tareas existentes

➕ Agregar nuevas tareas

✅ Marcar tareas como completadas

📊 Consultar estadísticas de progreso

⚙️ Adaptar comportamiento según el entorno (desarrollo o producción)

Cada entorno ajusta sus mensajes, límites y niveles de log según el Profile configurado.


---

## 🧩 Estructura del Proyecto

com.utn.tareas
├── model
│ ├── Tarea.java
│ └── Prioridad.java
├── repository
│ └── TareaRepository.java
├── service
│ ├── TareaService.java
│ ├── MensajeService.java
│ ├── MensajeDevService.java
│ └── MensajeProdService.java
└── TareasApplication.java


---

## ⚙️ Tecnologías Utilizadas

| Tecnología | Versión | Descripción |
|-------------|----------|-------------|
| ☕ Java | 17+ | Lenguaje principal |
| 🧩 Spring Boot | 3.x | Framework para backend |
| ⚙️ Maven | - | Gestión de dependencias |
| ✨ Lombok | - | Reducción de código boilerplate |
| 🔁 Spring Boot DevTools | - | Recarga automática durante desarrollo |

---

## 🚀 Cómo Ejecutar el Proyecto

Ejecutar con MAVEN -> mvn spring-boot:run

### 1️⃣ Clonar el repositorio

git clone https://github.com/usuario/tareas-springboot.git
cd tareas-springboot

🔧 Configuración de Profiles

El comportamiento de la aplicación se determina según el profile activo definido en el archivo:

📄 src/main/resources/application.properties

spring.profiles.active=dev  # o prod

🔹 Entorno DEV

Archivo: application-dev.properties

app.max-tareas=10
app.mostrar-estadisticas=true
logging.level.com.utn.tareas=DEBUG


✅ Mensajes detallados
📊 Estadísticas habilitadas
💻 Límite bajo de tareas

🔸 Entorno PROD

Archivo: application-prod.properties

app.max-tareas=1000
app.mostrar-estadisticas=false
logging.level.com.utn.tareas=ERROR


🚀 Mensajes simples
📉 Sin estadísticas
📈 Límite alto de tareas


## 📸 Capturas de pantalla de la consola con ambos profiles

Perfil de Produccion:
<img width="654" height="555" alt="{41469416-614F-423F-8C4A-FE885E9A9410}" src="https://github.com/user-attachments/assets/448e7180-7a39-459a-b1a4-0e403bf672a3" />

Perfil de Desarrollador:
<img width="646" height="621" alt="{63D8E219-5C16-410B-B428-9B7ECFA0F229}" src="https://github.com/user-attachments/assets/c3ac1d29-6163-4791-8986-702ed5a74d79" />

El desarrollo de este proyecto me permitió comprender en profundidad el ecosistema de Spring Boot y su relevancia en el desarrollo de aplicaciones modernas con Java.

La inyección de dependencias demostró ser clave para lograr un código modular, desacoplado y más fácil de mantener.

Por otro lado, la práctica con profiles y configuraciones externas permitió observar cómo un mismo proyecto puede adaptarse fácilmente a diferentes entornos (desarrollo y producción) sin alterar su código fuente.

Finalmente, el uso de anotaciones como @Service, @Repository y @Profile reforzó la importancia de las buenas prácticas, la organización del código y la claridad en la arquitectura del proyecto.

En conjunto, esta experiencia me brindó una visión más profesional y sólida sobre el desarrollo con Spring Boot.

##👤 Autor

Nicolas Andres Moreno Coll 
Legajo 50989
