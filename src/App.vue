<template>
  <div id="app">
    <b-navbar toggleable="lg" class="p-0" type="dark" variant="primary">
    <b-navbar-brand href="#"><img class="img-logo" src="./assets/img/logoNavWhite.png" alt="Logo institucional"></b-navbar-brand>

    <b-navbar-toggle target="nav-collapse"></b-navbar-toggle>

    <b-collapse id="nav-collapse" is-nav>  
      <!-- Right aligned nav items -->
      <b-navbar-nav class="ml-auto">
        <b-nav-item href="#">Inicio</b-nav-item>
        <b-nav-item href="#">Calendario</b-nav-item>
        <b-nav-item href="#">Contacto</b-nav-item>
        <b-nav-item-dropdown text="Ganancias" right>
          <b-dropdown-item href="#">Agregar gasto</b-dropdown-item>
          <b-dropdown-item href="#">Ver gasto</b-dropdown-item>
          <b-dropdown-item href="#">Ver ganancias</b-dropdown-item>
        </b-nav-item-dropdown>
        <b-nav-item-dropdown text="Turno" right>
          <b-dropdown-item href="#">Agendar turno</b-dropdown-item>
          <b-dropdown-item href="#">Ver turnos</b-dropdown-item>
        </b-nav-item-dropdown>
        <b-nav-item href="#">Ingresar</b-nav-item>
      </b-navbar-nav>
    </b-collapse>
  </b-navbar>
    <router-view/>
    <footer class="bg-primary">
      <div class="d-flex justify-content-around py-3">
        <p class="text-white m-auto">Derechos reservados &copy; 2023</p>
        <p class="text-white m-auto">Desarrollado por <a href="#" class="text-white text-yellow">FG-Fullstack</a></p>
      </div>
    </footer>
  </div>
</template>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  text-align: center;
  /* color: #2c3e50; */
}

/* nav {
  padding: 30px;
} */

nav a {
  font-weight: bold;
  /* color: #2c3e50; */
}
.nav-link {
  color: white !important;
}
.nav-link:hover {
  color: #f9fa5f !important;
  font-weight: normal;
}
.text-yellow:hover {
  color: #f9fa5f !important;
  font-weight: bold;
  text-decoration: none;
}
/* nav a.router-link-exact-active {
  color: #42b983;
} */
</style>
