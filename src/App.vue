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
      <a href="#perfil" class="profile-link">
        <div class="profile-icon-wrapper">
          <img src="https://img.icons8.com/?size=100&id=14736&format=png&color=000000" alt="Perfil" class="profile-icon" />
        </div>
      </a>
    </div>
  </nav>
</template>

<script lang="ts">
import { defineComponent } from 'vue';

export default defineComponent({});
</script>

<style scoped>
@import url('https://fonts.googleapis.com/css2?family=Poppins:wght@400;600&display=swap');

.navbar {
  display: flex;
  align-items: center;
  justify-content: space-between;
  padding: 0 2rem;
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
  color: #d41a23;
}

.navbar-profile {
  display: flex;
  align-items: center;
}

.profile-link {
  display: inline-block;
}

.profile-icon-wrapper {
  display: inline-block;
  border-radius: 50%;
  border: 2px solid #333;
  overflow: hidden;
  transition: transform 0.3s;
}

.profile-icon {
  width: 28px;
  height: 28px;
  display: block;
}

.profile-link:hover .profile-icon-wrapper {
  transform: scale(1.1);
}
</style>
