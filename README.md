📘 Proyecto Clon Universidad ECCI
Este proyecto es un clon institucional de la página de la Universidad ECCI, desarrollado con Vue 3 + Vite en el frontend y Express.js en el backend. Incluye secciones dinámicas como noticias, facilidades académicas, soluciones rápidas, comunidad unieccista, agenda universitaria y footer institucional.

⚠️ Nota importante:
Este proyecto es un clon académico/demostrativo.

No es la página oficial de la Universidad ECCI.

Algunos botones y enlaces no funcionan o no llevan a sitios oficiales.

Los accesos a servicios como Directorio Institucional, Preguntas Frecuentes, Portal Laboral, HCM, etc. son placeholders y no redirigen a las páginas reales.

Las imágenes utilizadas son placeholders (Picsum) y no corresponden a contenido oficial.

🚀 Tecnologías utilizadas
Frontend: Vue 3, Vite, CSS

Backend: Node.js, Express, CORS

Estilos: CSS modular + paleta institucional (azul #003366, amarillo #ffcc00, gris #f5f5f5)

Imágenes: Picsum (placeholder) + logo ECCI

📂 Estructura del proyecto
Código
ecci-clone/
 ├─ backend/
 │   └─ server.js
 └─ frontend/
     ├─ index.html
     ├─ vite.config.js
     ├─ package.json
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
⚙️ Instalación y ejecución
1. Clonar el repositorio
bash
git clone https://github.com/usuario/ecci-clone.git
cd ecci-clone
2. Backend
bash
cd backend
npm install
node server.js
El backend estará disponible en:
👉 http://localhost:3000

3. Frontend
bash
cd ../frontend
npm install
npm run dev
El frontend estará disponible en:
👉 http://localhost:5173

🧩 Funcionalidades principales
Navbar: Barra de navegación con logo institucional.

Slider: Carrusel de imágenes con transición animada.

Facilidades: Programas académicos por sede y ciclo.

Solutions: Accesos rápidos a servicios institucionales (no funcionales).

Community: Estadísticas de estudiantes, egresados y programas.

News: Noticias y artículos de actualidad por sede.

UniversityLife: Servicios y experiencias universitarias.

Agenda: Eventos académicos y fechas destacadas.

FooterInstitutional: Información legal, sedes y contactos.

📌 Limitaciones
Los botones y enlaces son demostrativos y no llevan a páginas oficiales.

El contenido (noticias, eventos, cifras) es simulado.

Las imágenes son placeholders y no corresponden a material institucional real.

✅ Resultado esperado
Al ejecutar el proyecto verás un clon institucional con:

Diseño completo desde el navbar hasta el footer.

Contenido dinámico en noticias y agenda.

Estilo coherente con la identidad visual de la Universidad ECCI.

Botones y enlaces no funcionales, ya que es un clon demostrativo.