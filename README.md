# Visual Case Study CMS

Este proyecto es un CMS de casos de estudio visuales construido con Vue.js 3, Express.js y MongoDB. Permite a los usuarios registrarse, iniciar sesión, crear estudios de casos mediante un editor visual de bloques y publicarlos en URLs únicas.

## Despliegue con Render

Haga clic en el botón para desplegar su propia copia en Render:

[![Deploy to Render](https://render.com/images/deploy-to-render-button.svg)](https://render.com/deploy?repo=https://github.com/sevepromx/visual-case-study-cms)

## Requisitos de entorno

Antes de ejecutar el proyecto localmente, necesitas crear un archivo `.env` en la carpeta `backend` con las siguientes variables:

```
MONGO_URI=mongodb+srv://<usuario>:<contraseña>@cluster/<base_de_datos>?retryWrites=true&w=majority
JWT_SECRET=su_clave_secreta
PORT=5000
```

## Pasos para ejecutar localmente

1. Clona este repositorio:
   ```
   git clone https://github.com/sevepromx/visual-case-study-cms.git
   cd visual-case-study-cms
   ```

2. Instala dependencias en el backend y frontend:
   ```
   cd backend
   npm install
   cd ../frontend
   npm install
   ```

3. Crea el archivo `.env` en `backend` con la URI de tu base de datos de MongoDB y un secreto JWT.

4. Ejecuta el backend:
   ```
   npm start
   ```

5. En otra terminal ejecuta el frontend:
   ```
   npm run dev
   ```

6. Abre `http://localhost:5173` en tu navegador para utilizar la aplicación.

## Estructura del proyecto

- `backend/` – API de Node.js con Express y Mongoose para autenticación y gestión de casos.
- `frontend/` – Aplicación de Vue.js con Vite, Pinia y Vue Router.
- `cms-casestudy.zip` – Archivo comprimido con todo el código fuente.
