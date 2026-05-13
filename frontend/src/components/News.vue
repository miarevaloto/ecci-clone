<template>
  <section class="news">
    <h2>Lo más reciente en la ECCI</h2>
    <p class="subtitle">Actualidad</p>

    <div class="tabs">
      <button v-for="city in cities" :key="city" @click="selectedCity = city" :class="{ active: selectedCity === city }">
        {{ city }}
      </button>
    </div>

    <div class="news-container">
      <div class="main-news">
        <img :src="mainNews.image" alt="principal" class="main-img" />
        <div class="main-content">
          <p class="date">{{ mainNews.date }} - {{ selectedCity }}</p>
          <h3>{{ mainNews.title }}</h3>
          <p>{{ mainNews.summary }}</p>
          <a href="#" class="link">Ver más →</a>
        </div>
      </div>

      <div class="sub-news">
        <div v-for="item in subNews" :key="item.title" class="sub-item">
          <img :src="item.image" alt="noticia" class="thumb" />
          <div>
            <p class="date">{{ item.date }} - {{ selectedCity }}</p>
            <h4>{{ item.title }}</h4>
            <a href="#" class="link">Ver más →</a>
          </div>
        </div>
      </div>
    </div>
  </section>
</template>

<script>
export default {
  data() {
    return {
      cities: ["Bogotá", "Cali", "Medellín"],
      selectedCity: "Bogotá",
      mainNews: {
        date: "29 de abril de 2026",
        title: "Más allá del «Prompt»: Por qué la Estrategia es el único diferencial real en el Mercadeo de 2026",
        summary:
          "En 2026, la pregunta ya no es si tu empresa usa Inteligencia Artificial, sino qué tan genérico se ha vuelto tu mensaje por culpa de ella. Con herramientas de IA al alcance de todos para generar contenido, segmentar audiencias y optimizar pautas, el mercado se ha inundado de campañas que «se ven bien» pero que no conectan.",
        image: "https://picsum.photos/800/500?random=21"
      },
      subNews: [
        {
          date: "29 de abril de 2026",
          title: "Dejar de «Apagar Incendios» para Empezar a Modelar: El Futuro de la Gerencia de Operaciones",
          image: "https://picsum.photos/300/200?random=22"
        },
        {
          date: "28 de abril de 2026",
          title: "Más allá de la reparación: Por qué la anticipación es la verdadera rentabilidad en 2026",
          image: "https://picsum.photos/300/200?random=23"
        },
        {
          date: "14 de abril de 2026",
          title: "5 sectores con alta demanda de ingenieros mecánicos en Colombia",
          image: "https://picsum.photos/300/200?random=24"
        },
        {
          date: "14 de abril de 2026",
          title: "Investigación desde la universidad: así funcionan los semilleros en la Universidad ECCI",
          image: "https://picsum.photos/300/200?random=25"
        }
      ]
    };
  }
};
</script>

<style scoped>
.news {
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
.news-container {
  display: flex;
  flex-wrap: wrap;
  gap: 2rem;
}
.main-news {
  flex: 1 1 60%;
  display: flex;
  gap: 1rem;
}
.main-img {
  width: 50%;
  border-radius: 8px;
  object-fit: cover;
}
.main-content {
  width: 50%;
}
.sub-news {
  flex: 1 1 35%;
  display: grid;
  grid-template-columns: 1fr;
  gap: 1rem;
}
.sub-item {
  display: flex;
  gap: 1rem;
  align-items: center;
}
.thumb {
  width: 100px;
  height: 70px;
  border-radius: 6px;
  object-fit: cover;
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
</style>
