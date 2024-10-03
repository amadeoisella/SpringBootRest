
## Spring Boot REST API

### 📄 Descripción del proyecto:

Este proyecto es una API REST desarrollada con Spring Boot que gestiona información sobre fabricantes (Maker) y productos (Product), permitiendo realizar operaciones CRUD en ambas entidades. El proyecto incluye la persistencia de datos en una base de datos MySQL, la inyección de datos iniciales mediante un archivo SQL, y la configuración de un entorno de desarrollo flexible.

### 🛠️ Herramientas utilizadas:

- Java 17: Lenguaje de programación.
- Spring Boot 3.3.4: Framework principal.
- spring-boot-starter-data-jpa: Persistencia de datos con JPA/Hibernate.
- spring-boot-starter-web: Creación de la API REST.
- spring-boot-devtools: Recarga automática en desarrollo.
- spring-boot-starter-test: Pruebas unitarias e integración.
- MySQL: Base de datos relacional.
- Lombok: Simplificación del código eliminando boilerplate.

### ⚙️ Configuración inicial

#### 🗄️ Base de datos:

El proyecto incluye un archivo import.sql en la carpeta src/main/resources para inyectar datos iniciales en la base de datos. La configuración de la conexión se encuentra en application.properties.

#### 🔧 Configuración del entorno:

Para clonar y ejecutar este proyecto, es necesario configurar el archivo application.properties con las credenciales de la base de datos:

#### 💾 Datos de conexión a la base de datos
- spring.datasource.url=jdbc:mysql://localhost:3306/rest_api_db
- spring.datasource.username=<tu_usuario>
- spring.datasource.password=<tu_contraseña>

Asegúrate de completar estos datos antes de ejecutar el proyecto.

### 🚀 Ejecución del proyecto

Sigue estos pasos para ejecutar el proyecto:

1. Clonar el repositorio.
2. Configurar las credenciales de MySQL en application.properties.
3. Ejecutar el proyecto usando Maven con el siguiente comando:

- mvn spring-boot:run

### 📝 Documentación de la API

Para consultar la documentación de la API y las pruebas con los distintos verbos HTTP usando Postman, accede a la siguiente URL:

[Documentación](https://documenter.getpostman.com/view/18266506/2sAXxLCa2K)

### 📌 Notas adicionales

- El proyecto usa spring.jpa.hibernate.ddl-auto=create-drop, por lo que la base de datos se crea y elimina en cada ejecución.
- Los datos iniciales se cargan automáticamente desde el archivo import.sql.
- Asegúrate de configurar correctamente el archivo application.properties con tus credenciales de la base de datos.