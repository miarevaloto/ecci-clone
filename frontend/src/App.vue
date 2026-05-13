<template>
  <div id="app">
    <Navbar />
    <Slider />
    <Facilidades />
    <Solutions />
    <Community />
    <News />
    <UniversityLife />
    <Agenda />
    <Footer />
  </div>
</template>

<script>
import Navbar from "./components/Navbar.vue";
import Slider from "./components/Slider.vue";
import Facilidades from "./components/Facilidades.vue";
import Solutions from "./components/Solutions.vue";
import Community from "./components/Community.vue";
import News from "./components/News.vue";
import UniversityLife from "./components/UniversityLife.vue";
import Agenda from "./components/Agenda.vue";
import Footer from "./components/Footer.vue";

export default {
  components: { Navbar, Slider, Facilidades, Solutions, Community, News, UniversityLife, Agenda, Footer }
};
</script>
