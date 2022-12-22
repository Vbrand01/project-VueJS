<template>
  <div>
    <primeiroComponente />
    <p>O dados de app é: {{ testando }}</p>
  </div>
</template>

<script>

  import primeiroComponente from './components/primeiroComponente.vue';

  export default{
    name: 'App',
    components: {
      primeiroComponente
    },
    data(){
      return{
        testando: 'teste'
      }
    }
  }
</script>