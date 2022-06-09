<template>
  <div class="side-bar">
    <div class="logo"><Logo/></div>
    <div class="said-main">
      <ul class="main">
        <li  class="visible" id="cero">
           <NuxtLink to="/apariencia">La Radio Viva </NuxtLink>
        </li>
        <li @click="openMenu1 = !openMenu1" class="visible" id="open" >La Marca
          <ul class="panel" v-show="openMenu1">
            <li class="invisibl" > <NuxtLink to="/novedades">Novedades </NuxtLink></li>
            <li class="invisibl" ><NuxtLink to="/figma">Figma </NuxtLink></li>
            <li class="invisibl"><NuxtLink to="/pdf">Pdf</NuxtLink></li>
          </ul>
        </li>
        <li  class="visible" id="cero">
           <NuxtLink to="/apariencia">APARIENCIA </NuxtLink>
        </li>
        <li @click="openMenu2 = !openMenu2" class="visible">BÁSICOS
          <ul class="panel" v-show="openMenu2">
            <li class="invisibl" > <NuxtLink to="/logotipos">Logotipos</NuxtLink></li>
            <li class="invisibl" > <NuxtLink to="/paletas">Paleta</NuxtLink></li>
            <li class="invisibl" > <NuxtLink to="/tipografia">Tipografía</NuxtLink></li>
            <li class="invisibl" > <NuxtLink to="/imagenes">Imágenes</NuxtLink></li>
            <li class="invisibl" > <NuxtLink to="/aplicaciones">Aplicaciones</NuxtLink></li>
          </ul>
        </li>
        <li @click="openMenu3 = !openMenu3" class="visible">RETÍCULAS
          <ul class="panel" v-show="openMenu3">
            <li class="invisibl" > <NuxtLink to="/base">Base</NuxtLink></li>
            <li class="invisibl" > <NuxtLink to="/aplicacion">Aplicación</NuxtLink></li>
          </ul>
        </li>
        <li @click="openMenu4 = !openMenu4" class="visible">NAVEGACIÓN
          <ul class="panel" v-show="openMenu4">
            <li class="invisibl" > <NuxtLink to="/iconos">Mapas</NuxtLink></li>
            <li class="invisibl" > <NuxtLink to="/botones">Low-fi + Mid-fi</NuxtLink></li>
          </ul>
        </li>
        <li @click="openMenu4 = !openMenu4" class="visible">COMPONENTES
          <ul class="panel" v-show="openMenu4">
            <li class="invisibl" > <NuxtLink to="/iconos">Iconos</NuxtLink></li>
            <li class="invisibl" > <NuxtLink to="/botones">Botones/Badge/Checkbox</NuxtLink></li>
            <li class="invisibl" > <NuxtLink to="/inputs">Inputs/Barras/Alerta</NuxtLink></li>
            <li class="invisibl" > <NuxtLink to="/tarjetas">Tarjetas</NuxtLink></li>
            <li class="invisibl" > <NuxtLink to="/formulario">Formularios/Portada</NuxtLink></li>
            <li class="invisibl" > <NuxtLink to="/formulario">Slides</NuxtLink></li>

        </ul>
        </li>
      </ul>
    </div>


  </div>
</template>
<script>
    export default {

    data(){
        return{
            openMenu1: false,
            openMenu2: false,
            openMenu3: false,
            openMenu4: false
        }
    }
    }
</script>

<style lang="postcss">
.side-bar{
    scroll-behavior: smooth;
     background-color: $blanco;
    width: 40vh;
    height: 100vh;
    position: fixed;
    box-shadow: $sombra1;
}
ul{
     font-size: 12pt;
      font-style: 400;
      color: $azul;
}
li{
     font-size: 12pt;
        font-style: 400;
        color: $azul;
        @apply ml-11 mt-8;
          
}
  #cero{
    margin-top: 0;
  }
    
</style>
