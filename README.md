# Currículum online — Javier Fulgencio López

Sitio web estático (HTML + CSS + JS, sin dependencias ni build) con el currículum
profesional, publicado con GitHub Pages.

## Estructura

```
curriculum-web/
├── index.html                                  Página principal
├── css/styles.css                              Estilos y tema claro/oscuro
├── js/main.js                                  Toggle de tema + animaciones
└── assets/
    ├── javier-fulgencio-lopez-cv.pdf           PDF descargable
    └── foto.jpg                                (opcional) fotografía de perfil
```

## Ver en local

Abrí `index.html` directamente en el navegador, o levantá un servidor local:

```bash
python3 -m http.server 8000
```

Y entrá a http://localhost:8000

## Añadir la fotografía

Copiá tu foto como `assets/foto.jpg`. Mientras no exista, se muestra un círculo
con las iniciales. No hace falta tocar el código.

## Publicar en GitHub Pages

```bash
git remote add origin git@github.com:<usuario>/<repo>.git
git push -u origin main
```

Luego, en el repositorio: **Settings → Pages → Source: Deploy from a branch →
Branch: `main` / `/ (root)` → Save**.

El sitio queda en `https://<usuario>.github.io/<repo>/`.

## Personalización rápida

- **Colores y tipografías**: variables CSS en `:root` y `[data-theme="dark"]` al
  inicio de `css/styles.css`.
- **Contenido**: editar directamente las secciones de `index.html`.
