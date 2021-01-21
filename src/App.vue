<template>
  <div class="app" >
    <Navbar/>
      <body>
        <transition name="transicion" mode="out-in">
          <router-view/>
        </transition>
      </body>
    <Footer/>
  </div>
</template>

<script>


import Navbar from '@/components/Navbar.vue'
import Footer from '@/components/Footer.vue'

export default {
  name: 'App',
    components: {
    Navbar,
    Footer
  },
}
</script>

<style>
body{
  background: url('./assets/fondo4.jpg');
  background-size: cover;
  background-repeat: no-repeat;
  height: auto;
}
.transicion-enter-active {
  transition:  all 1s ease;
}
.transicion-enter, .slide-fade-leave-to {
  transform: rotateY(100deg);
}
@import url('https://fonts.googleapis.com/css2?family=Acme&display=swap');
@import url('https://fonts.googleapis.com/css2?family=Lobster&display=swap');
</style>
