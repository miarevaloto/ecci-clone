<template>
  <div class="slider">
    <div
      v-for="(slide, index) in slides"
      :key="index"
      class="slide"
      :class="{ active: currentSlide === index, next: nextSlide === index }"
    >
      <img :src="slide.image" :alt="slide.title" />
      <div class="caption">
        <h2>{{ slide.title }}</h2>
        <p>{{ slide.text }}</p>
      </div>
    </div>
    <div class="controls">
      <button @click="prevSlide">‹</button>
      <button @click="nextSlideFn">›</button>
    </div>
  </div>
</template>

<script>
export default {
  data() {
    return {
      currentSlide: 0,
      nextSlide: null,
      slides: [
  {
    image: "https://picsum.photos/1350/600?random=11",
    title: "Campus moderno",
    text: "Instalaciones diseñadas para el aprendizaje."
  },
  {
    image: "https://picsum.photos/1350/600?random=12",
    title: "Estudiantes en clase",
    text: "Formación académica con visión global."
  },
  {
    image: "https://picsum.photos/1350/600?random=13",
    title: "Innovación tecnológica",
    text: "Impulsamos proyectos de investigación y desarrollo."
  }
]

    };
  },
  methods: {
    nextSlideFn() {
      this.nextSlide = (this.currentSlide + 1) % this.slides.length;
      setTimeout(() => {
        this.currentSlide = this.nextSlide;
        this.nextSlide = null;
      }, 800);
    },
    prevSlide() {
      this.nextSlide =
        (this.currentSlide - 1 + this.slides.length) % this.slides.length;
      setTimeout(() => {
        this.currentSlide = this.nextSlide;
        this.nextSlide = null;
      }, 800);
    }
  },
  mounted() {
    setInterval(() => {
      this.nextSlideFn();
    }, 5000);
  }
};
</script>

<style scoped>
.slider { position: relative; overflow: hidden; width: 100%; height: 600px; perspective: 1000px; }
.slide { position: absolute; width: 100%; height: 100%; opacity: 0; transform: translate3d(100%,0,0); transition: transform 0.8s ease, opacity 0.8s ease; }
.slide.active { opacity: 1; transform: translate3d(0,0,0); z-index: 2; }
.slide.next { opacity: 1; transform: translate3d(-100%,0,0); z-index: 1; }
.slide img { width: 100%; height: 600px; object-fit: cover; }
.caption { position: absolute; bottom: 40px; left: 60px; color: white; background: rgba(0,0,0,0.4); padding: 1rem 2rem; border-radius: 8px; animation: fadeInUp 1s ease; }
@keyframes fadeInUp { from { opacity: 0; transform: translateY(20px);} to { opacity: 1; transform: translateY(0);} }
.controls { position: absolute; bottom: 20px; right: 40px; }
button { background: #003366; color: white; border: none; padding: 0.5rem 1rem; margin: 0 0.3rem; cursor: pointer; border-radius: 4px; }
button:hover { background: #002244; }
</style>
