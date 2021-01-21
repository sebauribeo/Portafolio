<template>
    <div>
        <footer>
            <div class="footer">
                <div class="text-center">
                    <h3>Portafolio de: <strong>Sebastian Uribe</strong></h3>
                </div>
                <ul class="text-center">
                    <li><a href="https://www.linkedin.com/in/sebastian-uribe-o-64a81213b/" target="_blank"><font-awesome-icon class="icono fa-3x" :icon="['fab', 'linkedin']"></font-awesome-icon></a></li>
                    <li><a href="https://github.com/sebauribeo" target="_blank"><font-awesome-icon class="icono fa-3x" :icon="['fab', 'github-square']"></font-awesome-icon></a></li>
                    <li><a href="https://twitter.com/" target="_blank"><font-awesome-icon class="icono fa-3x" :icon="['fab', 'twitter-square']"></font-awesome-icon></a></li>
                </ul>
            </div>
        </footer>
    </div>
</template>

<script>
    export default {
        name: 'Footer',
    }
</script>

<style>
footer{
    background: linear-gradient(#d87300,#7c0080) ;
    position: relative;
    color: black;
    font-family: 'Lobster', cursive;
}
footer ul{
    padding: 0;
    margin: 0;
    text-decoration: none;
}
footer ul li{
    margin: 10px;
    display: inline;
}
.footer{
    display: grid;
    grid-template-columns: 1fr 1fr;
    grid-template-rows: 80px;
    align-items: center;
    justify-items: center;
}
@media(max-width: 450px){
    .footer{
        padding-top: 20px;
        display: grid;
        grid-template-columns: 1fr;
        grid-template-rows: 100px;
        align-items: center;
        justify-items: center;
    }
}
.icono{
  transition: 1s;  
  color: black;
}
.icono:hover{
  transform: scale(1.3);
  transition: 0.5s;
}
</style>