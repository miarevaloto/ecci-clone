📘 Proyecto Clon Universidad ECCI (Frontend)
Este proyecto es un clon institucional de la página de la Universidad ECCI, desarrollado con Vue 3 + Vite.
Incluye secciones dinámicas como noticias, facilidades académicas, soluciones rápidas, comunidad unieccista, agenda universitaria y footer institucional.

⚠️ Nota importante:
Este proyecto es un clon demostrativo.

No es la página oficial de la Universidad ECCI.

Algunos botones y enlaces no funcionan o llevan a enlaces aleatorios/demostrativos.

Las imágenes son placeholders (Picsum) y no corresponden a contenido oficial.

🚀 Tecnologías utilizadas
Framework: Vue 3 + Vite

Lenguaje: JavaScript (ES Modules)

Estilos: CSS modular + paleta institucional (azul #003366, amarillo #ffcc00, gris #f5f5f5)

Hosting: Vercel (Frontend)

📂 Estructura del proyecto
Código
frontend/
 ├─ index.html
 ├─ vite.config.js
 ├─ package.json
 ├─ .gitignore
 └─ src/
     ├─ main.js
     ├─ App.vue
     ├─ assets/
     │   └─ styles.css
     └─ components/
         ├─ Navbar.vue
         ├─ Slider.vue
         ├─ Facilidades.vue
         ├─ Solutions.vue
         ├─ Community.vue
         ├─ News.vue
         ├─ UniversityLife.vue
         ├─ Agenda.vue
         └─ FooterInstitutional.vue
⚙️ Instalación local
Clonar el repositorio:

bash
git clone https://github.com/TU_USUARIO/ecci-clone.git
cd ecci-clone/frontend
Instalar dependencias:

bash
npm install
Ejecutar en modo desarrollo:

bash
npm run dev
👉 La app estará disponible en http://localhost:5173

🧩 Scripts disponibles
npm run dev → inicia el servidor de desarrollo con Vite.

npm run build → genera la carpeta dist lista para producción.

npm run preview → sirve la carpeta dist localmente para pruebas.

📌 Configuración de .gitignore
El proyecto ya incluye un .gitignore que evita subir carpetas innecesarias:

Código
node_modules
dist
dist-ssr
*.log
.vscode/
.idea
.DS_Store
👉 Esto asegura que Vercel genere sus propios node_modules y dist durante el build.

🚀 Despliegue en Vercel
Subir a GitHub  
Asegúrate de que tu repositorio contenga el código fuente (src, public, package.json, vite.config.js) pero no node_modules ni dist.

Importar en Vercel

Inicia sesión en Vercel.

Haz clic en “Add New Project” → “Import Git Repository”.

Selecciona tu repositorio.

Configurar proyecto en Vercel

Framework Preset: Vite

Root Directory: frontend

Build Command: npm run build

Output Directory: dist

Deploy automático  
Vercel instalará dependencias, construirá el proyecto y publicará tu clon en una URL pública:

Código
https://ecci-clone.vercel.app
Actualizaciones  
Cada vez que hagas git push a GitHub, Vercel reconstruirá y desplegará automáticamente la nueva versión.

✅ Resultado esperado
Tu clon estará disponible públicamente en Vercel.

El diseño completo desde el navbar hasta el footer institucional será visible.

Los botones iniciales tendrán funciones básicas (scroll interno o enlaces demostrativos).

El README aclara que es un clon y que algunos botones no llevan a páginas oficiales.
