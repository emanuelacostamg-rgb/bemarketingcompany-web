# Be Marketing Company - Sitio Web

Sitio web oficial de Be Marketing Company, agencia de marketing digital.

## 🚀 Despliegue en Cloudflare Pages (Paso a Paso)

### Paso 1: Subir a GitHub
1. Entra a [github.com](https://github.com) e inicia sesión.
2. Haz clic en el botón **"New"** (Nuevo) o "+" arriba a la derecha.
3. Nombre del repositorio: `bemarketingcompany-web`
4. Déjalo en **Public**.
5. Haz clic en **"Create repository"**.
6. En la siguiente pantalla, busca el enlace que dice **"uploading an existing file"**.
7. Arrastra y suelta TODOS los archivos y carpetas de tu proyecto (`index.html`, `css`, `js`, `assets`, `sitemap.xml`, `robots.txt`, `README.md`).
8. Abajo, escribe un mensaje como "Subida inicial del sitio web" y haz clic en **"Commit changes"**.

### Paso 2: Conectar con Cloudflare Pages
1. Entra a [dash.cloudflare.com](https://dash.cloudflare.com) e inicia sesión.
2. En el menú de la izquierda, haz clic en **"Workers & Pages"**.
3. Haz clic en el botón **"Create application"** y luego en la pestaña **"Pages"**.
4. Haz clic en **"Connect to Git"**.
5. Autoriza a Cloudflare para acceder a tu cuenta de GitHub (si te lo pide).
6. Busca y selecciona tu repositorio: `bemarketingcompany-web`.
7. En "Configure your project":
   - **Production branch**: `main` (o `master`)
   - **Build command**: Déjalo **vacío** (es solo HTML/CSS/JS, no necesita compilación).
   - **Build output directory**: Déjalo **vacío** (o pon `/`).
8. Haz clic en **"Save and Deploy"**.

### Paso 3: Configurar tu dominio
1. Una vez que termine el despliegue (tarda ~30 segundos), verás una URL temporal (ej: `bemarketingcompany-web.pages.dev`).
2. Haz clic en **"Custom domains"** en el menú del proyecto.
3. Haz clic en **"Set up a custom domain"**.
4. Escribe: `bemarketing.company` y haz clic en **"Continue"**.
5. Cloudflare te pedirá confirmar que eres el dueño del dominio. Sigue las instrucciones en pantalla (normalmente es agregar unos registros DNS en donde compraste el dominio).

¡Listo! Tu sitio estará en vivo en `https://bemarketing.company`.