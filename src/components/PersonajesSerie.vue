<template>
  <div id="app">
    <div class="pipol">
      <img :src="datos.src" :alt="datos.nombre" class="imagen" />
      <p>{{ datos.nombre }}</p>
    </div>
  </div>
</template>

<script>
export default {
  props: {
    datos: {
      type: Object,
    },
  },
}
</script>

<style scoped>

 .pipol{
   width: 100%;
   padding: 40px;
   font-size: 40px;
   
 }

  
.imagen {
  border-radius: 50%;
  position: relative;
}
</style>
