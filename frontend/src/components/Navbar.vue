<template>
  <nav class="navbar">
    <img src="/logo-ecci.png" alt="Logo ECCI" class="logo" />
    <ul>
      <li>
        <button @click="goToUniversity('Inicios', 'https://es.wikipedia.org/wiki/Universidad')">Inicio</button>
      </li>
      <li>
        <button @click="goToUniversity('Programas de Ingeniería', 'https://www.google.com/search?q=PROGRAMAS+DE+INGENIERIA+EN+COLOMBIA&oq=PROGRAMAS+DE+INGENIERIA+EN+COLOMBIA&gs_lcrp=EgZjaHJvbWUyBggAEEUYOdIBCTEyNzM1ajBqN6gCALACAA&sourceid=chrome&ie=UTF-8')">Programas</button>
      </li>
      <li>
        <button @click="goToUniversity('Noticias Universidades Bogota', 'https://www.google.com/search?q=noticias+universidades+en+bogota+colombia&sca_esv=e1aed3f059b28a74&biw=1920&bih=953&sxsrf=ANbL-n6OAMdotlLHFgivcxGAZ_tNKymeXA%3A1778859549131&ei=HT4HatnBB7WXwbkPuLij2Qw&oq=noticias+universidades+en+bogota&gs_lp=Egxnd3Mtd2l6LXNlcnAiIG5vdGljaWFzIHVuaXZlcnNpZGFkZXMgZW4gYm9nb3RhKgIIATIFECEYoAEyBRAhGKABMgUQIRifBTIFECEYnwUyBRAhGJ8FMgUQIRifBUiMNFCtCljOJXABeAGQAQCYAZQBoAHhDaoBBDAuMTS4AQPIAQD4AQGYAg-gApoOwgIKEAAYRxjWBBiwA8ICBhAAGBYYHsICCBAAGIAEGKIEwgIFEAAY7wWYAwCIBgGQBgiSBwQxLjE0oAeRNLIHBDAuMTS4B5YOwgcGMC4xMi4zyAcigAgB&sclient=gws-wiz-serp')">Noticias</button>
      </li>
      <li>
        <button @click="goToUniversity('Contactos', 'https://www.google.com/search?q=contactos+universidades&sca_esv=e1aed3f059b28a74&sxsrf=ANbL-n6W78zWzNwiCh7stXyQ4mX2g3kNDQ:1778859651784&udm=1&lsack=gz4Hat6yL4T8wbkP-O6N8Qs&sa=X&ved=2ahUKEwiegJnN0LuUAxUEfjABHXh3I74QjGp6BAgsEAA&biw=1920&bih=953&dpr=1')">Contacto</button>
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
