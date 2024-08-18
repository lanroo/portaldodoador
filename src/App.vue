<template>
  <nav class="navbar">
    <div class="navbar-brand">
      <img src="./assets/logo.png" alt="Portal do Doador" class="navbar-logo" />
    </div>
    <ul class="navbar-menu">
      <li class="navbar-item"><a href="#noticias">Notícias</a></li>
      <li class="navbar-item"><a href="#contato">Contato</a></li>
      <li class="navbar-item"><a href="#voluntariado">Voluntariado</a></li>
      <li class="navbar-item"><a href="#projetos">Projetos</a></li>
    </ul>
    <div class="navbar-profile">
      <Button icon="pi pi-user" class="p-button-rounded p-button-secondary" />
    </div>
  </nav>
</template>

<script lang="ts">
import { defineComponent } from 'vue';
import Button from 'primevue/button';

export default defineComponent({
  components: {
    Button,
  },
});
</script>

<style scoped>
@import url('https://fonts.googleapis.com/css2?family=Poppins:wght@400;600&display=swap');

.navbar {
  display: flex;
  align-items: center;
  justify-content: space-between;
  padding: 1rem 2rem;
  background-color: #ffffff;
  box-shadow: 0 2px 4px rgba(0, 0, 0, 0.1);
  font-family: 'Poppins', sans-serif;
}

.navbar-logo {
  width: 120px;
}

.navbar-menu {
  list-style: none;
  display: flex;
  gap: 2rem;
  margin: 0;
  padding: 0;
}

.navbar-item a {
  text-decoration: none;
  color: #333;
  font-weight: 600;
}

.navbar-item a:hover {
  color: #007bff;
}

.navbar-profile {
  display: flex;
  align-items: center;
}
</style>
