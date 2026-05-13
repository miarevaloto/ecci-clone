<template>
  <section class="solutions">
    <div class="solutions-grid">
      <div class="solution" v-for="item in items" :key="item.title">
        <img :src="item.icon" alt="icon" class="icon"/>
        <p>{{ item.title }}</p>
      </div>
    </div>
  </section>
</template>

<script>
export default {
  data() {
    return {
      items: [
        { title: "Centro de Servicios - Bogotá", icon: "https://cdn-icons-png.flaticon.com/512/684/684908.png" },
        { title: "FPQRS", icon: "https://cdn-icons-png.flaticon.com/512/1828/1828640.png" },
        { title: "Atención Telefónica - (601) 3537171", icon: "https://cdn-icons-png.flaticon.com/512/597/597177.png" },
        { title: "Preguntas Frecuentes", icon: "https://cdn-icons-png.flaticon.com/512/1828/1828817.png" },
        { title: "Directorio Institucional", icon: "https://cdn-icons-png.flaticon.com/512/1077/1077063.png" },
        { title: "Sedes", icon: "https://cdn-icons-png.flaticon.com/512/684/684908.png" }
      ]
    };
  }
};
</script>

<style scoped>
.solutions { padding: 2rem; background: #f5f5f5; }
.solutions-grid { display: grid; grid-template-columns: repeat(auto-fit, minmax(200px, 1fr)); gap: 1rem; }
.solution { background: white; border-radius: 8px; padding: 1rem; text-align: center; box-shadow: 0 2px 4px rgba(0,0,0,0.1); }
.icon { width: 40px; margin-bottom: 0.5rem; }
</style>
