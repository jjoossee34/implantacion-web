Práctica WordPress con Docker Compose
1. Descripción del proyecto

En esta práctica se despliega WordPress utilizando Docker Compose. El proyecto utiliza dos servicios: WordPress como gestor de contenidos y MySQL como base de datos.

2. Tecnologías utilizadas
Docker
Docker Compose
WordPress
MySQL 8.0
3. Estructura del proyecto
docker-compose.yml: archivo de configuración de los servicios y volúmenes.
README.md: documentación del proyecto.
4. Configuración

El archivo docker-compose.yml define dos servicios:

wordpress: ejecuta WordPress y publica el puerto 8080 del equipo en el puerto 80 del contenedor.
db: ejecuta MySQL 8.0 y configura la base de datos exampledb.

Se utilizan volúmenes para conservar los archivos de WordPress y los datos de MySQL.

5. Cómo ejecutar el proyecto
Abrir una terminal en la carpeta del proyecto.
Comprobar la configuración:
docker compose config

Iniciar los contenedores:
docker compose up -d

Acceder a WordPress desde el navegador:

http://localhost:8080

6. Cómo detener el proyecto

Para detener los contenedores, ejecutar:

docker compose down


Este comando detiene y elimina los contenedores, pero conserva los volúmenes.

7. Volúmenes
wordpress: almacena los archivos de WordPress.
db: almacena los datos de MySQL.