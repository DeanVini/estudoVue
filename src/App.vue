<template>
  <NavBar/>

  <MultipleEvents/>
  
  <primeiroComponente/>
  
  <lifeCycle/>
  
  <pessoa/>

  <Comment/>

</template>

<script>
  import primeiroComponente from './components/primeiroComponente.vue';
  import lifeCycle from './components/lifeCycle.vue';
  import pessoa from './components/pessoa.vue';
  import NavBar from './components/NavBar.vue';
  import Comment from './components/Comment.vue';
  import MultipleEvents from './components/MultipleEvents.vue';


  export default {
    name: 'App',
    components: {
      NavBar,
      primeiroComponente,
      lifeCycle,
      pessoa,
      Comment,
      MultipleEvents
    }
  }

</script>
