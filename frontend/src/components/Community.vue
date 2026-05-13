<template>
  <section class="community">
    <h2>Nuestra comunidad unieccista</h2>
    <div class="stats">
      <div v-for="stat in stats" :key="stat.label" class="stat">
        <h3>{{ stat.value }}</h3>
        <p>{{ stat.label }}</p>
      </div>
    </div>
    <img src="https://upload.wikimedia.org/wikipedia/commons/2/21/Colombia_location_map.svg" alt="Mapa Colombia" class="map"/>
  </section>
</template>

<script>
export default {
  data() {
    return {
      stats: [
        { label: "Sedes", value: "3" },
        { label: "Estudiantes", value: "16.000" },
        { label: "Egresados", value: "65.000" },
        { label: "Pregrados", value: "31" },
        { label: "Especializaciones", value: "7" },
        { label: "Maestrías", value: "6" },
        { label: "Doctorado", value: "1" }
      ]
    };
  }
};
</script>

<style scoped>
.community { background: #ffcc00; color: #003366; padding: 2rem; text-align: center; border-radius: 8px; }
.stats { display: flex; flex-wrap: wrap; justify-content: center; gap: 2rem; margin-top: 1rem; }
.stat h3 { font-size: 2rem; margin: 0; }
.map { width: 300px; margin-top: 2rem; }
</style>
