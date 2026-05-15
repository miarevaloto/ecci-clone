# 🎓 Clon Universidad ECCI (Frontend)

[![Vue.js](https://img.shields.io/badge/Vue.js-3.x-4FC08D?logo=vue.js&logoColor=white)](https://vuejs.org/)
[![Vite](https://img.shields.io/badge/Vite-5.x-646CFF?logo=vite&logoColor=white)](https://vitejs.dev/)
[![JavaScript](https://img.shields.io/badge/JavaScript-ES6+-F7DF1E?logo=javascript&logoColor=black)](https://developer.mozilla.org/en-US/docs/Web/JavaScript)
[![Vercel](https://img.shields.io/badge/Vercel-Deployed-000000?logo=vercel&logoColor=white)](https://vercel.com)

> **Proyecto demostrativo** - Clon institucional de la página de la Universidad ECCI, desarrollado con Vue 3 + Vite.

🌐 **Demo en vivo:** [ecci-clone.vercel.app](https://ecci-clone.vercel.app)

---

## ✨ Características principales

- 🎯 **Diseño fiel**: réplica de la interfaz institucional con paleta oficial  
- 📱 **Responsive**: adaptación a móviles, tablets y escritorio  
- 🧩 **Componentes modulares**: arquitectura Vue reutilizable  
- ⚡ **Rendimiento optimizado**: Vite para builds rápidos y hot-reload  
- 🎨 **Paleta institucional**: Azul `#003366`, Amarillo `#ffcc00`, Gris `#f5f5f5`  

---

## 📌 Secciones implementadas

- ✅ Barra de navegación institucional  
- ✅ Slider/Carrusel principal  
- ✅ Noticias destacadas  
- ✅ Facilidades académicas  
- ✅ Soluciones rápidas  
- ✅ Comunidad Unieccista  
- ✅ Agenda universitaria  
- ✅ Footer institucional completo  

---

## ⚠️ Aviso importante

Este es un **clon demostrativo** con fines educativos y de portafolio.  
- ❌ No es la página oficial de la Universidad ECCI  
- 🔗 Algunos botones y enlaces son demostrativos o direccionan a URLs genéricas  
- 🖼️ Las imágenes provienen de [Picsum](https://picsum.photos/) como placeholders  

---

## 🚀 Tecnologías utilizadas

| Tecnología | Descripción |
|------------|-------------|
| **[Vue 3](ca://s?q=Aprender_más_sobre_Vue_3)** | Framework progresivo de JavaScript |
| **[Vite](ca://s?q=Qué_es_Vite)** | Build tool y servidor de desarrollo |
| **[JavaScript ES6+](ca://s?q=Características_de_JavaScript_ES6)** | Lógica de componentes |
| **CSS Scoped** | Estilos encapsulados por componente |
| **[Vercel](ca://s?q=Cómo_funciona_Vercel)** | Hosting y despliegue continuo |

---

## 📁 Estructura del proyecto

```plaintext
frontend/
├─ index.html              # Punto de entrada HTML
├─ vite.config.js          # Configuración de Vite
├─ package.json            # Dependencias y scripts
├─ .gitignore              # Archivos ignorados por Git
└─ src/
   ├─ main.js              # Punto de entrada de la app
   ├─ App.vue              # Componente raíz
   ├─ assets/              # Recursos estáticos
   │  └─ styles.css        # Estilos globales
   └─ components/          # Componentes Vue reutilizables
      ├─ Navbar.vue        # Barra de navegación
      ├─ Slider.vue        # Carrusel principal
      ├─ Facilidades.vue   # Sección de facilidades
      ├─ Solutions.vue     # Soluciones rápidas
      ├─ Community.vue     # Comunidad Unieccista
      ├─ News.vue          # Noticias destacadas
      ├─ UniversityLife.vue# Vida universitaria
      ├─ Agenda.vue        # Agenda universitaria
      └─ FooterInstitutional.vue # Pie de página
⚙️ Instalación y uso local
Prerrequisitos
Node.js (v18 o superior)

npm o yarn

Pasos de instalación
bash
# 1. Clonar el repositorio
git clone https://github.com/TU_USUARIO/ecci-clone.git

# 2. Acceder al directorio
cd ecci-clone/frontend

# 3. Instalar dependencias
npm install

# 4. Iniciar servidor de desarrollo
npm run dev
🔥 La aplicación estará disponible en http://localhost:5173

📜 Scripts disponibles
Comando	Descripción
npm run dev	Inicia servidor de desarrollo con hot-reload
npm run build	Genera build de producción en dist/
npm run preview	Previsualiza el build de producción localmente


🚢 Despliegue en Vercel
1️⃣ Sube tu código a GitHub
2️⃣ Importa el proyecto en Vercel  
3️⃣ Configuración recomendada:

Framework Preset: Vite

Root Directory: frontend

Build Command: npm run build

Output Directory: dist
4️⃣ ¡Listo! Vercel generará una URL pública como:
👉 https://ecci-clone.vercel.app

🔄 Cada git push activará un nuevo despliegue automático.

🎯 Resultado esperado
✅ Interfaz completa desde navbar hasta footer

✅ Diseño responsive y fiel al institucional

✅ Botones con funcionalidades básicas (scroll interno o enlaces demostrativos)

✅ Disponible públicamente en Vercel

📄 Licencia
Este proyecto es de uso educativo y demostrativo.
No está afiliado oficialmente con la Universidad ECCI.

🙌 Créditos
Desarrollado como proyecto de portafolio utilizando Vue 3 + Vite.

🌐 Demo en vivo: ecci-clone.vercel.app

📂 Repositorio: github.com/miarevaloto/ecci-clone

⭐ ¡Si te gusta este proyecto, no olvides darle una estrella en GitHub!
