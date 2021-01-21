<template>
  <div class="container">

    <div class="row">
      <div class="container__animacion col-12 col-sm-12 col-md-6 col-lg-6 col-xl-6 mt-2">
        <div class="animacion row">
          <img class="object col-6 " data-value="-3" v-b-tooltip.bottom.hover title="SASS" src="../assets/SASS.png" alt="imagen">
          <img class="object col-6 " data-value="3" v-b-tooltip.bottom.hover title="HTML" src="../assets/HTML.png" alt="imagen">
          <img class="object col-6 " data-value="3" v-b-tooltip.bottom.hover title="Bootstrap" src="../assets/Bootstrap.png" alt="imagen">
          <img class="object col-6 " data-value="-3" v-b-tooltip.bottom.hover title="CSS" src="../assets/CSS.png" alt="imagen">
          <img class="object col-6 " data-value="-3" v-b-tooltip.bottom.hover title="JavaScript" src="../assets/JS.png" alt="imagen">
          <img class="object col-6 " data-value="3" v-b-tooltip.bottom.hover title="VueJs" src="../assets/VUE.png" alt="imagen">

        </div>

      </div>

  <div class="mt-5 p-3 col-12 col-sm-12 col-md-6 col-lg-6 col-xl-6">
    <h3 class="text-danger"><font-awesome-icon class="text-danger" :icon="['fab', 'html5']"></font-awesome-icon> HTML</h3>
    <b-progress :value="80" variant="danger" ></b-progress>
    <h3 class="text-info"><font-awesome-icon class="text-info" :icon="['fab', 'css3-alt']"></font-awesome-icon> CSS</h3>
    <b-progress :value="70" variant="info" ></b-progress>
    <h3 class="text-danger"><font-awesome-icon class="text-danger" :icon="['fab', 'sass']"></font-awesome-icon> SASS</h3>
    <b-progress :value="50" variant="danger" ></b-progress>
    <h3 class="text-primary"><font-awesome-icon class="text-primary" :icon="['fab', 'bootstrap']"></font-awesome-icon> Bootstrap</h3>
    <b-progress :value="80" variant="primary" ></b-progress>
    <h3 class="text-warning"><font-awesome-icon class="text-warning" :icon="['fab', 'js-square']"></font-awesome-icon> Javascript</h3>
    <b-progress :value="65" variant="warning" ></b-progress>
    <h3 class="text-success"><font-awesome-icon class="text-success" :icon="['fab', 'vuejs']"></font-awesome-icon> VueJS</h3>
    <b-progress :value="65" variant="success" ></b-progress>
  </div>

    </div>
    
  </div>
</template>

<script type="text/javascript">
        document.addEventListener("mousemove", parallax);
        function parallax(e){
          document.querySelectorAll(".object").forEach(function(move){
        
            var moving_value = move.getAttribute("data-value");
            var x = (e.clientX * moving_value)/100;
            var y = (e.clientY * moving_value)/100;
        
            move.style.transform = "translateX(" + x + "px) translateY(" + y + "px)";
          })
        }
    export default {
        name: 'Skills',
    }
</script>

<style scoped>
.container{
  top: 50px;
  margin-bottom: 100px;
  background: rgba(0, 0, 0, 0.856);
  position: relative;
  border-radius: 25px;
  padding: 40px;
}
.container__animacion{
  margin: 0;
  padding: 0;
  display: flex;
  justify-content: center;
  align-items: center;
}
.animacion{
  width: 400px;
  height: 400px;
  background: linear-gradient(45deg, black,rgb(28, 145, 153),  black);
  border-radius: 50%;
  border: 10px solid rgb(209, 212, 25);
  box-shadow: 0 0 10px white;

}
.animacion img{
  width: 100px;
  height: 100px;
}

</style>