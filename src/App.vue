<template>
  <div id="app">
    <Navbar />
    <LandingPage />
    <About />
    <Menu />
    <Footer />
  </div>
</template>

<script>
import Navbar from './components/Navbar.vue'
import LandingPage from './components/LandingPage.vue'
import About from './components/About.vue'
import Menu from './components/Menu.vue'
import Footer from './components/Footer.vue'

export default {
  name: 'App',
  components: {
    Navbar,
    LandingPage,
    About,
    Menu,
    Footer
  },
}
</script>

<style>
@import url("https://fonts.googleapis.com/css2?family=Open+Sans&display=swap");

* {
 margin: 0px;
 padding: 0px;
 box-sizing: border-box;
}

html, body{
  font-family: 'Open Sans';
}
.container-col {
    display: flex;
    flex-direction: column;
    height: 100vh;
    width: 100vw;
}

.container-row{
  display: flex;
  flex-direction: row;
  width: 100vw;
  height: 100vh;
  align-items: center;
}
</style>
