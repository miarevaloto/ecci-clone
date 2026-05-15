<template>
  <nav class="navbar">
    <img src="/logo-ecci.png" alt="Logo ECCI" class="logo" />
    <ul>
      <li>
        <button @click="goToUniversity('Inicios', 'https://es.wikipedia.org/wiki/Universidad')">Inicio</button>
      </li>
      <li>
        <button @click="goToUniversity('Programas de Ingeniería', 'https://www.google.com/search?q=PROGRAMAS+DE+INGENIERIA+EN+COLOMBIA')">Programas</button>
      </li>
      <li>
        <button @click="goToUniversity('Noticias Universidades Bogota', 'https://www.google.com/search?q=noticias+universidades+en+bogota')">Noticias</button>
      </li>
      <li>
        <!-- Aquí cambiamos la acción: en vez de abrir URL, mostramos el modal -->
        <button @click="showContactForm = true">Contacto</button>
      </li>
    </ul>
  </nav>

  <!-- Modal emergente -->
  <div v-if="showContactForm" class="modal-overlay">
    <div class="modal">
      <h2>Formulario de Contacto</h2>
      <form @submit.prevent="submitForm">
        <label>
          Nombre:
          <input type="text" v-model="contact.name" required />
        </label>
        <label>
          Correo:
          <input type="email" v-model="contact.email" required />
        </label>
        <label>
          Mensaje:
          <textarea v-model="contact.message" required></textarea>
        </label>
        <div class="actions">
          <button type="submit">Enviar</button>
          <button type="button" @click="showContactForm = false">Cerrar</button>
        </div>
      </form>
    </div>
  </div>
</template>

<script>
export default {
  data() {
    return {
      showContactForm: false,
      contact: {
        name: "",
        email: "",
        message: ""
      }
    };
  },
  methods: {
    goToUniversity(name, url) {
      alert(`Redirigiendo a ${name}...`);
      window.open(url, "_blank");
    },
    submitForm() {
      alert(`Gracias ${this.contact.name}, tu mensaje ha sido enviado.`);
      this.showContactForm = false;
      // Aquí podrías agregar lógica para enviar los datos a un backend
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

/* Estilos del modal */
.modal-overlay {
  position: fixed;
  top: 0;
  left: 0;
  width: 100%;
  height: 100%;
  background: rgba(0,0,0,0.6);
  display: flex;
  align-items: center;
  justify-content: center;
}
.modal {
  background: #fff;
  padding: 2rem;
  border-radius: 8px;
  width: 400px;
  max-width: 90%;
}
.modal h2 {
  margin-bottom: 1rem;
}
.modal label {
  display: block;
  margin-bottom: 1rem;
}
.modal input, .modal textarea {
  width: 100%;
  padding: 0.5rem;
  margin-top: 0.3rem;
  border: 1px solid #ccc;
  border-radius: 4px;
}
.actions {
  display: flex;
  justify-content: space-between;
  margin-top: 1rem;
}
</style>
