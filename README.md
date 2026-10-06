# Portafolio de Alejandra Melo

Sitio estático de una sola página. No necesita instalación ni compilación.

## Estructura

- `index.html`: toda la página (contenido, estilos y scripts).
- `media/`: videos, imágenes y logos.
- `.nojekyll`: le indica a GitHub Pages que sirva los archivos tal cual.

## Publicar en GitHub Pages

1. Crea un repositorio nuevo en GitHub. Si lo llamas `TU-USUARIO.github.io`, el sitio queda en esa dirección; con cualquier otro nombre queda en `TU-USUARIO.github.io/NOMBRE-DEL-REPO`.
2. Sube **el contenido** de esta carpeta a la raíz del repositorio (`index.html`, `media/`, `.nojekyll`, `README.md`). Desde la web: "Add file" > "Upload files" y arrastra todo. O por terminal:

   ```bash
   git init
   git add .
   git commit -m "Portafolio de Alejandra Melo"
   git branch -M main
   git remote add origin https://github.com/TU-USUARIO/NOMBRE-DEL-REPO.git
   git push -u origin main
   ```
3. En el repositorio: Settings > Pages > "Build and deployment" > Source: "Deploy from a branch" > Branch: `main`, carpeta `/ (root)` > Save.
4. Espera uno o dos minutos y abre la dirección que muestra esa misma pantalla.

## Dependencias externas

La página carga desde internet las fuentes (Google Fonts) y la librería de scroll suave Lenis (unpkg). Si alguna no carga, el sitio sigue funcionando con fuentes del sistema y scroll normal.

## Editar contenido

- Los textos están en español dentro de `index.html`. La traducción al inglés está en el objeto `ES_EN` del script, al final del archivo: si cambias un texto en español, cambia también su clave ahí.
- Para reemplazar un video o imagen, guarda el archivo nuevo en `media/` con el mismo nombre.
