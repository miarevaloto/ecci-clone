<template>
  <nav class="navbar">
    <img src="/logo-ecci.png" alt="Logo ECCI" class="logo" />
    <ul>
      <li>
        <button @click="goToUniversity('Harvard', 'https://www.harvard.edu')">Inicio</button>
      </li>
      <li>
        <button @click="goToUniversity('Programas de Ingeniería', 'https://www.google.com/search?q=PROGRAMAS+DE+INGENIERIA+EN+COLOMBIA&oq=PROGRAMAS+DE+INGENIERIA+EN+COLOMBIA&gs_lcrp=EgZjaHJvbWUyBggAEEUYOdIBCTEyNzM1ajBqN6gCALACAA&sourceid=chrome&ie=UTF-8')">Programas</button>
      </li>
      <li>
        <button @click="goToUniversity('MIT News', 'https://news.mit.edu')">Noticias</button>
      </li>
      <li>
        <button @click="goToUniversity('UNAL Contacto', 'https://unal.edu.co/contacto')">Contacto</button>
      </li>
    </ul>
  </nav>
</template>

<script>
export default {
  methods: {
    goToUniversity(name, url) {
      alert(`Redirigiendo a ${name}...`);
      window.open(url, "_blank");
    }
  }
};
</script>

<style scoped>
.navbar {
  display: flex;
  align-items: center;
  justify-content: space-between;
  background: #003366;
  padding: 1rem;
}
.logo {
  height: 40px;
}
ul {
  list-style: none;
  display: flex;
  gap: 1rem;
}
button {
  background: #ffcc00;
  border: none;
  padding: 0.5rem 1rem;
  border-radius: 6px;
  cursor: pointer;
  font-weight: 600;
  color: #003366;
}
button:hover {
  background: #e6b800;
}
</style>
