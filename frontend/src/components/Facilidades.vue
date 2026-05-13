<template>
  <section class="programs">
    <h2>Encuentra el programa que hará brillar tu talento</h2>
    <div class="tabs">
      <button v-for="city in cities" :key="city" @click="selectedCity = city" :class="{ active: selectedCity === city }">
        {{ city }}
      </button>
    </div>

    <div v-if="selectedCity === 'Bogotá'" class="program-list">
      <div class="cycle">
        <h3>Ciclo I</h3>
        <ul>
          <li>Tecnología en Gestión Gastronómica</li>
          <li>Tecnología en Producción de Moda</li>
          <li>Tecnología en Mercadeo y Diseño Publicitario</li>
          <li>Tecnología en Gestión de Comercio Exterior</li>
        </ul>
      </div>
      <div class="cycle">
        <h3>Ciclo II</h3>
        <ul>
          <li>Profesional de Gastronomía</li>
          <li>Profesional de Diseño en Modas</li>
          <li>Profesional en Mercadeo y Publicidad</li>
          <li>Profesional en Contaduría Pública</li>
          <li>Profesional en Comercio Internacional</li>
          <li>Profesional en Ingeniería Mecánica</li>
          <li>Profesional en Ingeniería Industrial</li>
        </ul>
      </div>
      <div class="cycle">
        <h3>Ciclo único</h3>
        <ul>
          <li>Profesional en Entrenamiento Deportivo</li>
          <li>Profesional en Enfermería</li>
          <li>Profesional en Lenguas Modernas</li>
          <li>Profesional en Derecho</li>
          <li>Profesional en Estadística</li>
        </ul>
      </div>
    </div>
  </section>
</template>

<script>
export default {
  data() {
    return {
      cities: ["Bogotá", "Cali", "Medellín"],
      selectedCity: "Bogotá"
    };
  }
};
</script>

<style scoped>
.programs { padding: 2rem; background: #fff; border-radius: 8px; box-shadow: 0 2px 4px rgba(0,0,0,0.1); }
.tabs { display: flex; gap: 1rem; margin-bottom: 1rem; }
.tabs button { background: #e6e6e6; border: none; padding: 0.5rem 1rem; cursor: pointer; border-radius: 4px; }
.tabs button.active { background: #003366; color: white; }
.cycle { margin-bottom: 1rem; }
.cycle h3 { color: #003366; }
</style>
