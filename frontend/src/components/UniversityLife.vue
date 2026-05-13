<template>
  <section class="university-life">
    <h2>Vive la Universidad</h2>
    <p class="subtitle">Aquí encontrarás todo lo que necesitas para vivir una experiencia universitaria completa.</p>

    <div class="cards">
      <div v-for="item in items" :key="item.title" class="card">
        <img :src="item.image" :alt="item.title" />
        <div class="card-footer">{{ item.title }}</div>
      </div>
    </div>
  </section>
</template>

<script>
export default {
  data() {
    return {
      items: [
        { title: "Bienestar Universitario", image: "https://picsum.photos/400/300?random=31" },
        { title: "Biblioteca", image: "https://picsum.photos/400/300?random=32" },
        { title: "Becas y Descuentos", image: "https://picsum.photos/400/300?random=33" },
        { title: "Internacionalización", image: "https://picsum.photos/400/300?random=34" },
        { title: "Prácticas y Pasantías", image: "https://picsum.photos/400/300?random=35" },
        { title: "Portal Laboral", image: "https://picsum.photos/400/300?random=36" },
        { title: "Ciclo Coterminal", image: "https://picsum.photos/400/300?random=37" },
        { title: "Egresados", image: "https://picsum.photos/400/300?random=38" }
      ]
    };
  }
};
</script>

<style scoped>
.university-life {
  padding: 2rem;
  background: #fff;
  border-radius: 8px;
  box-shadow: 0 2px 4px rgba(0,0,0,0.1);
}
.subtitle {
  color: #666;
  margin-bottom: 1rem;
}
.cards {
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
  gap: 1rem;
}
.card {
  position: relative;
  overflow: hidden;
  border-radius: 8px;
  box-shadow: 0 2px 6px rgba(0,0,0,0.1);
}
.card img {
  width: 100%;
  height: 200px;
  object-fit: cover;
}
.card-footer {
  background: #003366;
  color: white;
  text-align: center;
  padding: 0.5rem;
  font-weight: 500;
}
</style>
