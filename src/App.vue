<template>
  <primeiroComponente/>

  <lifeCycle/>
  
  <Picture/>
  
  <pessoa/>

</template>

<script>
  import primeiroComponente from './components/primeiroComponente.vue';
  import lifeCycle from './components/lifeCycle.vue';
  import pessoa from './components/pessoa.vue';
  import Picture from './components/picture.vue'; 


  export default {
    name: 'App',
    components: {
      primeiroComponente,
      lifeCycle,
      pessoa,
      Picture
    }
  }

</script>