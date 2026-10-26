# StudySwap

Plataforma web para que estudiantes universitarios compartan apuntes, ganen créditos y se conecten con tutores pares.

Este repositorio contiene un **prototipo de frontend** sin dependencias: HTML, CSS y JavaScript puros. Los datos se guardan en `localStorage`, así que cada navegador tiene su propia copia.

## Funciones
- Registro simple de usuario (10 créditos iniciales)
- Catálogo con búsqueda y filtros por facultad, materia y valoración
- Vista previa difuminada y adquisición con créditos
- Publicación de apuntes (+2 créditos) y reseñas de 1 a 5 estrellas
- Perfil de tutor y reserva de sesiones pagadas con créditos
- Modo claro y oscuro automático

## Cómo ejecutarlo
Abre `index.html` en el navegador. No requiere instalación.

## Publicarlo en GitHub Pages
1. Sube todos los archivos a un repositorio.
2. En **Settings → Pages**, elige la rama `main` y la carpeta `/ (root)`.
3. Tu sitio quedará en `https://TU-USUARIO.github.io/NOMBRE-DEL-REPO/`.

## Estructura
```
index.html
css/styles.css
js/app.js
```

## Siguientes pasos (backend real)
Según el diseño técnico original:
- API con Node.js/Express o FastAPI, autenticación con JWT y contraseñas con hash
- PostgreSQL (por ejemplo con Supabase) con las tablas `users`, `subjects`, `notes` y `reviews`
- Almacenamiento de archivos PDF e imágenes (Supabase Storage o S3) y vista previa de páginas
- Endpoints: `POST /api/auth/register`, `POST /api/auth/login`, `GET/POST /api/notes`, `GET /api/notes/:id`, `POST /api/notes/:id/download`
- Calendario de tutorías

## Licencia
MIT
