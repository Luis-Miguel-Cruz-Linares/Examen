<template>
  <Grid>
      <img :src="url" :alt="nombre">
      <h2>{{ nombre }}</h2> 
      <h4>{{ descripcion }}</h4>
      <h3>{{ costo }}</h3>
      <a :href="url" target="_blank">Ordenar</a>
  </Grid>
</template>

<script>
  import Grid from "./Grid.vue";
  export default{
  props: {
      url: {
          String,
      },
      nombre: {
          String,
      },
      descripcion: {
          String,
      },
      costo: {
          String,
      },
  },
  components: { Grid },
};
</script>

<style scopet>

  img{
      width: 8  rem;
      height: 8rem;
      padding: 0.5rem;
      background:aqua;
      border-radius: 30px;
  }
  a{
      text-decoration: none;
      color: rgb(41, 206, 123);
      background: black;
      padding: 0.3rem;
      border-radius: 5px;
      border: 1px solid #ffffff;
      margin-bottom: 60px;
  }
  
</style>