Aplicación Web para Validación de Circulación de Pico y Placa

Descripción del Proyecto

Este proyecto consiste en una aplicación web para validar la circulación vehicular según las restricciones de pico y placa. Se utiliza Java 21 para el backend y Angular 19 para el frontend, proporcionando una interfaz moderna y un backend robusto.

Repositorios

Backend

Código fuente: https://github.com/cpiguave/picoyplaca_backend.git

Despliegue (JAR): https://github.com/cpiguave/picoyplaca_backend_deploy.git

Frontend

Código fuente: https://github.com/cpiguave/picoyplaca_frontend.git

Despliegue (dist): https://github.com/cpiguave/picoyplaca_frontend_deploy.git

Despliegue de la Aplicación

Requisitos Previos para el Despliegue

Backend

Servidor: Asegúrese de tener un servidor con Java 21 instalado.

Herramientas de Construcción: Maven o Gradle configurado.

Contenedor Opcional: Docker instalado (si se utiliza para el despliegue).

Frontend

Servidor Web: Servidor compatible con aplicaciones Angular, como NGINX o Apache.

Node.js: (v16 o superior) para la construcción del proyecto.

Pasos para el Despliegue

Backend

Clonar el repositorio de despliegue:

git clone https://github.com/cpiguave/picoyplaca_backend_deploy.git

Ejecutar el archivo JAR disponible:

java -jar Backend_picoyplaca-0.0.1-SNAPSHOT.jar

Opcional: Configurar un servicio en el sistema para que el backend se ejecute automáticamente al iniciar el servidor.

Frontend

Clonar el repositorio de despliegue:

git clone https://github.com/cpiguave/picoyplaca_frontend_deploy.git

Copiar los archivos en la carpeta dist/ al servidor web (NGINX o Apache).

Configurar el servidor web para servir la aplicación Angular:

En NGINX, agregar una configuración similar:

server {
    listen 80;
    server_name ejemplo.com;
    root /ruta/a/dist/;

    location / {
        index index.html;
        try_files $uri /index.html;
    }
}

Verificación

Acceder al dominio o dirección IP configurada para verificar que la aplicación esté funcionando correctamente.

Probar la conectividad entre el frontend y el backend.

Uso de la Aplicación

Ingresar al dominio configurado para la aplicación.

Ingresar el número de placa , fecha y hora para verificar las restricciones de circulación.
