# React Hola Mundo

Este es un proyecto básico de React.js que muestra un simple "Hola Mundo". Incluye un Dockerfile y un workflow de GitHub Actions para la automatización del proceso de construcción y despliegue.

## Instalación

1. Clona este repositorio.
2. Instala las dependencias:
   ```bash
   npm install
   ```
3. Inicia la aplicación:
   ```bash
   npm start
   ```

## Uso con Docker

1. Construye la imagen:
   ```bash
   docker build -t react-hola-mundo .
   ```
2. Ejecuta el contenedor:
   ```bash
   docker run -p 3000:3000 react-hola-mundo
   ```

## Workflow de GitHub Actions

El archivo `docker-react.yml` automatiza la construcción y publicación de la imagen en Docker Hub. Asegúrate de configurar los secretos `DOCKER_USERNAME` y `DOCKER_PASSWORD` en tu repositorio.
