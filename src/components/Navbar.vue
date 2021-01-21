<template>
  <div>
      <b-navbar toggleable="lg" type="dark" variant="faded" class="nav">
        <b-navbar-brand>
          <router-link to="/">
            <b-iconstack class="logo ml-4" font-scale="4">
              <b-icon class="icono-1" stacked icon="code-slash" scale="0.75"></b-icon>
              <b-icon class="icono-2" stacked icon="circle"></b-icon>
            </b-iconstack>
          </router-link>
        </b-navbar-brand>
        <b-navbar-toggle target="nav-collapse"></b-navbar-toggle>
        <b-collapse class="nav__collapse" id="nav-collapse" is-nav>
          <b-navbar-nav class="ml-auto">
            <b-nav-item class="m-0 p-0"><router-link class="h3 mx-3" to="/">Inicio</router-link></b-nav-item>
            <b-nav-item class="m-0 p-0"><router-link class="h3 mx-3" to="/skills">Skills</router-link></b-nav-item>
            <b-nav-item class="m-0 p-0"><router-link class="h3 mx-3" to="/proyectos">Proyectos</router-link></b-nav-item>
          </b-navbar-nav>
        </b-collapse>
      </b-navbar>


  </div>
</template>

<script>
export default {
  name: 'Navbar',
}
</script>

<style scoped lang="scss">
  .logo{
    transition: 2s;
    margin: 0;
  }
  .logo:hover{
    transform: rotate(360deg);
    color: red;
    transition: 2s;
  }
  .nav{
    width: 100%;
    background: linear-gradient(#89ffd8, rgb(3, 53, 59)) ;
  }
  .icono-1{
    font-weight: 800;
    color: black;
  }
  .icono-2{
    color: yellow;
  }
a{
  color: black;
  background-color: transparent;
  font-family: 'Lobster', cursive;
}
a:hover{
  transform: scale(1.1);
  text-decoration: none;
  color: #f3410b;
}

</style>
