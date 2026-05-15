<template>
  <section class="agenda">
    <h2>Unieccista, conoce tu agenda universitaria</h2>
    <p class="subtitle">Eventos</p>

    <div class="tabs">
      <button v-for="city in cities" :key="city" @click="selectedCity = city" :class="{ active: selectedCity === city }">
        {{ city }}
      </button>
    </div>

    <div class="events">
      <div v-for="event in events" :key="event.title" class="event-card">
        <img :src="event.image" :alt="event.title" />
        <div class="event-content">
          <p class="date">{{ event.date }} - {{ selectedCity }}</p>
          <h3>{{ event.title }}</h3>
          <p>{{ event.description }}</p>
          <a href="#" class="link">Ver más →</a>
        </div>
      </div>
    </div>

    <div class="center">
      <button class="btn" @click="goToUniversity('Eventos', 'https://www.google.com/search?q=eventos+universidades&oq=eventos+universidades&gs_lcrp=EgZjaHJvbWUyBggAEEUYOdIBCDQ3NjdqMGo3qAIAsAIA&sourceid=chrome&ie=UTF-8">Ver más eventos</button>
    </div>
  </section>
</template>

<script>
export default {
  data() {
    return {
      cities: ["Bogotá", "Cali", "Medellín"],
      selectedCity: "Bogotá",
      events: [
        {
          date: "23 Julio",
          title: "V Encuentro de Investigación en Lenguas Modernas, Marketing e Interculturalidad",
          description: "Encuentro académico para compartir experiencias pedagógicas y proyectos de investigación.",
          image: "https://picsum.photos/800/400?random=41"
        },
        {
          date: "23 Julio",
          title: "Open Day Virtual Posgrados",
          description: "Conoce la oferta académica de posgrados virtuales y oportunidades de crecimiento profesional.",
          image: "https://picsum.photos/800/400?random=42"
        },
        {
          date: "15 Julio",
          title: "Open Day Presencial de Posgrados",
          description: "Evento presencial para profesionales y egresados interesados en programas de posgrado.",
          image: "https://picsum.photos/800/400?random=43"
        }
      ]
    };
},
methods: {
    goToUniversity(name, url) {
      alert(`Redirigiendo a ${name}...`);
      window.open(url, "_blank");
    }
  }
};
</script>

<style scoped>
.agenda {
  padding: 2rem;
  background: #fff;
  border-radius: 8px;
  box-shadow: 0 2px 4px rgba(0,0,0,0.1);
}
.subtitle {
  color: #666;
  margin-bottom: 1rem;
}
.tabs {
  display: flex;
  gap: 1rem;
  margin-bottom: 1rem;
}
.tabs button {
  background: #e6e6e6;
  border: none;
  padding: 0.5rem 1rem;
  cursor: pointer;
  border-radius: 4px;
}
.tabs button.active {
  background: #003366;
  color: white;
}
.events {
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
  gap: 1.5rem;
}
.event-card {
  background: #fafafa;
  border-radius: 8px;
  overflow: hidden;
  box-shadow: 0 2px 6px rgba(0,0,0,0.1);
}
.event-card img {
  width: 100%;
  height: 200px;
  object-fit: cover;
}
.event-content {
  padding: 1rem;
}
.date {
  font-size: 0.8rem;
  color: #666;
}
.link {
  color: #ffcc00;
  text-decoration: none;
  font-weight: 500;
}
.link:hover {
  text-decoration: underline;
}
.center {
  text-align: center;
  margin-top: 2rem;
}
.btn {
  background: #ffcc00;
  color: #003366;
  border: none;
  padding: 0.8rem 1.5rem;
  border-radius: 6px;
  font-weight: 600;
  cursor: pointer;
}
.btn:hover {
  background: #e6b800;
}
</style>
