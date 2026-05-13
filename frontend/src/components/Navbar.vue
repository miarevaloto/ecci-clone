<template>
  <nav class="navbar">
    <img src="/logo-ecci.png" alt="Logo ECCI" class="logo"/>
    <ul>
      <li><a href="#">Inicio</a></li>
      <li><a href="#">Programas</a></li>
      <li><a href="#">Noticias</a></li>
      <li><a href="#">Contacto</a></li>
    </ul>
  </nav>
</template>

<style scoped>
.navbar {
  background-color: #003366;
  padding: 1rem 2rem;
  display: flex;
  align-items: center;
  justify-content: space-between;
}
.logo {
  height: 50px;
}
.navbar ul {
  display: flex;
  list-style: none;
  gap: 2rem;
  margin: 0;
}
.navbar a {
  color: white;
  text-decoration: none;
  font-weight: 500;
}
.navbar a:hover {
  border-bottom: 2px solid #ffcc00;
}
</style>
