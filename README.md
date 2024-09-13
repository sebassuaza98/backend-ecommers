Especificaciones técnicas del proyecto:

Java: 17
Spring Boot: 3.3.0
Maven: 3.0
MySQL: 8.0
Prerequisitos:

MySQL 8.0
Maven 3.0
JDK 17
Editor de texto (VSCode) o IDE preferido
Docker
Configuración de Docker y Maven:

Docker: Instrucciones de instalación
Maven: Instrucciones de instalación
JDK 17: Instrucciones de instalación
Repositorio del proyecto: El proyecto backend se encuentra desplegado en un contenedor Docker. El repositorio Git está a continuación: https://github.com/sebassuaza98/backend-ecommers.git

Nota: Asegúrate de tener Docker instalado y en funcionamiento.

Clonación del repositorio: Una vez clonado el repositorio, abre tu IDE de preferencia, el proyecto y en la raíz del proyecto ejecuta el comando:

bash
Copiar código
docker-compose build
Este comando se utiliza para construir la imagen de Docker.

Iniciar los servicios: Ejecuta el comando para iniciar los servicios:

bash
Copiar código
docker-compose up
Ejecución local: Si deseas ejecutar el proyecto de forma local, luego de haber clonado el repositorio, en la carpeta raíz, ejecuta el comando para limpiar e instalar las dependencias necesarias:

bash
Copiar código
mvn clean install
Manual de usuario: Se adjunta en el correo electrónico el manual de usuario sobre cómo consumir las peticiones.

Activar la API: Para activar la API y consumir los servicios, ejecuta:

bash
Copiar código
.\mvnw.cmd spring-boot:run
Errores comunes y solución:

Error de conexión a la base de datos: Verifica la configuración en application.properties y asegúrate de que MySQL esté en ejecución.
Problemas con Docker: Asegúrate de que Docker esté instalado y en ejecución. Revisa los logs para obtener más detalles.
Ejemplo de uso: Una vez que la API esté en funcionamiento, puedes realizar peticiones HTTP a los endpoints proporcionados en el manual de usuario para interactuar con el backend.
