# 🎓 Clon Universidad ECCI (Frontend)

[![Vue.js](https://img.shields.io/badge/Vue.js-3.x-4FC08D?logo=vue.js&logoColor=white)](https://vuejs.org/)
[![Vite](https://img.shields.io/badge/Vite-5.x-646CFF?logo=vite&logoColor=white)](https://vitejs.dev/)
[![JavaScript](https://img.shields.io/badge/JavaScript-ES6+-F7DF1E?logo=javascript&logoColor=black)](https://developer.mozilla.org/en-US/docs/Web/JavaScript)
[![Vercel](https://img.shields.io/badge/Vercel-Deployed-000000?logo=vercel&logoColor=white)](https://vercel.com)

> **Proyecto demostrativo** - Clon institucional de la página de la Universidad ECCI, desarrollado con Vue 3 + Vite.

![Vista previa del proyecto](https://via.placeholder.com/1200x600/003366/ffffff?text=Universidad+ECCI+Clone)

## ✨ Características

- 🎯 **Diseño fiel** - Réplica de la interfaz institucional con paleta de colores oficial
- 📱 **Responsive** - Adaptación a diferentes tamaños de pantalla
- 🧩 **Componentes modulares** - Arquitectura basada en componentes Vue reutilizables
- ⚡ **Rendimiento optimizado** - Uso de Vite para builds rápidos y hot-reload
- 🎨 **Paleta institucional** - Azul `#003366`, amarillo `#ffcc00`, gris `#f5f5f5`

### Secciones implementadas

- ✅ Barra de navegación institucional
- ✅ Slider/Carrusel principal
- ✅ Noticias destacadas
- ✅ Facilidades académicas
- ✅ Soluciones rápidas
- ✅ Comunidad Unieccista
- ✅ Agenda universitaria
- ✅ Footer institucional completo

## ⚠️ Aviso importante

> Este es un **clon demostrativo** con fines educativos y de portafolio.
>
> - ❌ No es la página oficial de la Universidad ECCI
> - 🔗 Algunos botones y enlaces son demostrativos o direccionan a URLs aleatorias
> - 🖼️ Las imágenes son placeholder de [Picsum](https://picsum.photos/) y no representan contenido oficial

## 🚀 Tecnologías utilizadas

| Tecnología | Descripción |
|------------|-------------|
| **Vue 3** | Framework progresivo de JavaScript |
| **Vite** | Build tool y servidor de desarrollo |
| **JavaScript (ES Modules)** | Lógica de componentes |
| **CSS Modular** | Estilos encapsulados por componente |
| **Vercel** | Hosting y despliegue continuo |

## 📁 Estructura del proyecto

## 📁 Estructura del proyecto

| Ruta | Descripción |
|------|-------------|
| `frontend/` | Raíz del proyecto frontend |
| ├─ `index.html` | Punto de entrada HTML |
| ├─ `vite.config.js` | Configuración de Vite |
| ├─ `package.json` | Dependencias y scripts |
| ├─ `.gitignore` | Archivos ignorados por Git |
| └─ `src/` | Código fuente principal |
| &nbsp;&nbsp;&nbsp;&nbsp;├─ `main.js` | Punto de entrada de la app |
| &nbsp;&nbsp;&nbsp;&nbsp;├─ `App.vue` | Componente raíz |
| &nbsp;&nbsp;&nbsp;&nbsp;├─ `assets/` | Recursos estáticos |
| &nbsp;&nbsp;&nbsp;&nbsp;│&nbsp;&nbsp;&nbsp;&nbsp;└─ `styles.css` | Estilos globales |
| &nbsp;&nbsp;&nbsp;&nbsp;└─ `components/` | Componentes Vue reutilizables |
| &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;├─ `Navbar.vue` | Barra de navegación |
| &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;├─ `Slider.vue` | Carrusel principal |
| &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;├─ `Facilidades.vue` | Sección de facilidades |
| &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;├─ `Solutions.vue` | Soluciones rápidas |
| &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;├─ `Community.vue` | Comunidad Unieccista |
| &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;├─ `News.vue` | Noticias destacadas |
| &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;├─ `UniversityLife.vue` | Vida universitaria |
| &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;├─ `Agenda.vue` | Agenda universitaria |
| &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;└─ `FooterInstitutional.vue` | Pie de página |

## ⚙️ Instalación y uso local

### Prerrequisitos

- Node.js (versión 18 o superior)
- npm o yarn

### Pasos de instalación

# 1. Clonar el repositorio
git clone https://github.com/TU_USUARIO/ecci-clone.git

# 2. Acceder al directorio del frontend
cd ecci-clone/frontend

# 3. Instalar dependencias
npm install

# 4. Iniciar servidor de desarrollo
npm run dev
La aplicación estará disponible en http://localhost:5173 🔥

📜 Scripts disponibles
Comando	Descripción
npm run dev	Inicia servidor de desarrollo con hot-reload
npm run build	Genera build de producción en dist/
npm run preview	Previsualiza el build de producción localmente
🚢 Despliegue en Vercel
Configuración automática
Sube tu código a GitHub

git add .
git commit -m "Initial commit"
git push origin main
Importa el proyecto en Vercel

Ve a vercel.com

Click en "Add New" → "Project"

Selecciona tu repositorio

Configuración recomendada

Parámetro	Valor
Framework Preset	Vite
Root Directory	frontend
Build Command	npm run build
Output Directory	dist
¡Listo! Vercel generará una URL como:

https://ecci-clone.vercel.app
Actualizaciones automáticas
Cada git push a tu repositorio activará un nuevo despliegue automático en Vercel. 🔄

📝 .gitignore incluido
gitignore
node_modules/
dist/
dist-ssr/
*.log
.vscode/
.idea/
.DS_Store
🎯 Resultado esperado
✅ Interfaz completa desde navbar hasta footer

✅ Diseño responsive y fiel al institucional

✅ Botones con funcionalidades básicas (scroll interno o enlaces demostrativos)

✅ Disponible públicamente en Vercel

📄 Licencia
Este proyecto es de uso educativo y demostrativo. No está afiliado oficialmente con la Universidad ECCI.

🙌 Créditos
Desarrollado como proyecto de portafolio utilizando Vue 3 y Vite.

Demo en vivo: https://ecci-clone.vercel.app
Repositorio: github.com/TU_USUARIO/ecci-clone

⭐ ¡Si te gusta este proyecto, no olvides darle una estrella en GitHub!

## 🔧 Mejoras realizadas

1. **Header visual** - Añadidos badges tecnológicos y un banner de vista previa
2. **Tablas** - Para mostrar scripts y configuraciones de forma más clara
3. **Emojis y iconos** - Mejoran la legibilidad visual
4. **Estructura jerárquica** - Uso consistente de `##`, `###` y `---`
5. **Código resaltado** - Bloques `bash` y `gitignore` con sintaxis correcta
6. **Sección de créditos** - Links de demo y repositorio
7. **Llamada a la acción** - Estrella de GitHub al final
8. **Información en columnas** - Para tecnologías y configuraciones

Simplemente reemplaza `TU_USUARIO` con tu nombre de usuario de GitHub y el README estará listo para impresionar en tu repositorio. ¿Necesitas que ajuste algún detalle más?
