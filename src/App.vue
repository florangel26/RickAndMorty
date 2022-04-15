<template>

  <div id="app">
    <div class="titulo">
      <h1 class="h1">Rick and Morty</h1>
       </div>
   
        <PersonajesSerie v-for="(character, index) in characters" :key="index" :datos="character"/>
          
           </div>
</template>

<script>
import PersonajesSerie from './components/PersonajesSerie.vue'

export default {
  name: 'app',
  components: {
    PersonajesSerie,
  },
  data() {
    return {
      characters: [
        {
          nombre: 'Rick Sanchez',
          src: 'https://rickandmortyapi.com/api/character/avatar/1.jpeg',
        },
        {
          nombre: 'Morty Smith',
          src: 'https://rickandmortyapi.com/api/character/avatar/2.jpeg',
        },
        {
          nombre: 'Summer Smith',
          src: 'https://rickandmortyapi.com/api/character/avatar/3.jpeg',
        },
        {
          nombre: 'Beth Smith',
          src: 'https://rickandmortyapi.com/api/character/avatar/4.jpeg',
        },
        {
          nombre: 'Jerry Smith',
          src: 'https://rickandmortyapi.com/api/character/avatar/5.jpeg',
        },
        {
          nombre: 'Abadango Cluster Princess',
          src: 'https://rickandmortyapi.com/api/character/avatar/6.jpeg',
        },
      ],
    }
  },
}
</script>

<style>
body{
 background-image: url('https://rickandmortypod.com/wp-content/uploads/2018/11/cropped-RM_page-header_background1-3.png');
  background-size: cover;
  background-repeat: no-repeat;
}
#app {
  font-family: 'Shadows Into Light', cursive;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;

  color: #03f153;
}
.titulo{
 padding-top: 50px;
 text-align: center;
}
.h1{
 font-size: 70px;


}

</style>
