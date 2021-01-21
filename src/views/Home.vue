<template>
  <div class="container">
    <div class="row">
      <div class="col-12 col-sm-12 col-md-6 col-lg-6 col-xl-6">
        <img src="#" alt="">
      </div >
      <div class="col-12 col-sm-12 col-md-6 col-lg-6 col-xl-6">
        <h2>Soy<strong> Sebastian Uribe</strong>, Chef de profesión por un poco más de 15 años y actualmente reinventando mi carrera hacia la programacion, en estos momentos estoy egresado del bootcamp 'Front End (VueJs)' que imparte Desafío Latam y próximamente en marzo comenzaré a perfeccionar mis conocimientos en Ingeniería en informática.</h2>
      </div>

    </div>

  </div>
</template>

<script>


export default {
  name: 'Home',

}
</script>

<style scoped>
.container{
  top: 50px;
  background: rgba(0, 0, 0, 0.856);
  border-radius: 25px;
  position: relative;
  height: auto;
  margin-bottom: 100px;
}
h2{
  color: white;
  font-family: 'Acme', sans-serif;
  padding: 10px;
  margin: 50px 0;
}
strong{
  color: rgb(255, 145, 0);
}
img{
  background: linear-gradient(45deg, black,rgb(28, 145, 153),  black);
  width: 100%;
  height: 400px;
  padding: 40px;
  margin: 50px 0;
  border-radius: 50%;
  border: 10px solid rgb(209, 212, 25);
  display: flex;
  justify-content: center;
  align-items: center;
  position: relative;
  box-shadow: 0 0 10px white;

}


 
</style>