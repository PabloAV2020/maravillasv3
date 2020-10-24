<template>
  <div id="app">
    <Navigation
    :nav-links="navLinks"
    background="#fff"
    link-color="#777"
    />
    <div id="nav">
      <router-link to="/">Inicio</router-link> |
      <router-link to="/about">Acerca de</router-link>
      <router-link to="/services">Servicios</router-link>
      <router-link to="/gallery">Galería</router-link>
      <router-link to="/contact">Contacto</router-link>
    </div>
    <router-view/>
    <div>
      <webapp-footer/>
    </div>
  </div>
</template>

<script>
import footer from './components/Footer.vue'
import Navigation from './components/Navigation.vue'

export default {
  name: 'App',
  components: {
    'webapp-footer':footer,
    Navigation
  },
  data: () => ({
    navLinks: [
      {
        text: 'Inicio',
		path: '/',
      },
      {
        text: 'Acerca de',
		path: '/about',
      },
      {
        text: 'Servicios',
		path: '/services',
      },
      {
        text: 'Galeria',
		path: '/gallery',
      },
      {
        text: 'Contacto',
		path: '/contact',
      }
    ]
  })
}

</script>


<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  background: green;
}

#nav {
  padding: 30px;
}

#nav a {
  font-weight: bold;
  color: #2c3e50;
}

#nav a.router-link-exact-active {
  color: #42b983;
}
</style>
