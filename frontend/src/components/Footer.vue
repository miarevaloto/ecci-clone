<template>
  <footer class="footer-institutional">
    <div class="social">
      <p>Síguenos en nuestras redes:</p>
      <div class="icons">
        <i class="fab fa-facebook"></i>
        <i class="fab fa-instagram"></i>
        <i class="fab fa-youtube"></i>
        <i class="fab fa-linkedin"></i>
        <i class="fab fa-tiktok"></i>
      </div>
    </div>

    <div class="footer-content">
      <div class="column">
        <img src="/logo-ecci.png" alt="Logo ECCI" class="logo" />
        <p>Universidad ECCI | Vigilada Mineducación</p>
        <p>Reconocimiento como Universidad: Resolución No. 13370 de 19 de Agosto de 2014.</p>
        <p>© Derechos Reservados Universidad ECCI – Fundada en 1977</p>

        <p><strong>Correo Electrónico Notificaciones judiciales</strong><br />
        notificaciones.judiciales@ecci.edu.co</p>

        <p><strong>Correo Electrónico de Atención al ciudadano</strong><br />
        info@ecci.edu.co</p>
      </div>

      <div class="column">
        <h3>SEDES</h3>
        <p><strong>BOGOTÁ</strong><br />Carrera 19 # 49 - 20<br />Localidad de Teusaquillo</p>
        <p><strong>CALI</strong><br />Av 4 Norte No. 13N - 03</p>
        <p><strong>MEDELLÍN</strong><br />Calle 49 # 45 - 65</p>
      </div>

      <div class="column">
        <h3>EXPLORA LA UNIVERSIDAD</h3>
        <ul>
          <li><a href="#">Nosotros</a></li>
          <li><a href="#">Normatividad</a></li>
          <li><a href="#">Transparencia y acceso a la información pública</a></li>
          <li><a href="#">Ingresa a HCM</a></li>
        </ul>
      </div>
    </div>
  </footer>
</template>

<style scoped>
.footer-institutional {
  background-color: #003366;
  color: white;
  padding: 2rem;
  font-size: 0.9rem;
}
.social {
  display: flex;
  justify-content: space-between;
  align-items: center;
  border-bottom: 1px solid #004080;
  padding-bottom: 1rem;
  margin-bottom: 1rem;
}
.icons i {
  margin: 0 0.5rem;
  font-size: 1.2rem;
  cursor: pointer;
}
.footer-content {
  display: flex;
  flex-wrap: wrap;
  justify-content: space-between;
  gap: 2rem;
}
.column {
  flex: 1 1 30%;
}
.column h3 {
  color: #ffcc00;
  margin-bottom: 0.5rem;
}
.column a {
  color: #ffcc00;
  text-decoration: none;
}
.column a:hover {
  text-decoration: underline;
}
.logo {
  width: 160px;
  margin-bottom: 1rem;
}
</style>
