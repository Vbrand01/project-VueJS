<template>
  <div class="container">
    <Header />

    <div class="componentes">
    <PrimeiroComponente />
    <p>pirmeiro componente criado</p>
    <hr>
    <h3>O dados de app é: {{ testando }}</h3>
    <hr>
    <LifeCycle />
    <p>Usando LifeCycle</p>
    <hr>
    <Pessoa />
    <p>Repartindo componentes</p>  
  </div>

  </div>
  
  
</template>

<script>

  import Header from './components/Header.vue'
  import PrimeiroComponente from './components/PrimeiroComponente.vue';
  import LifeCycle from './components/LifeCycle.vue';
  import Pessoa from './components/Pessoa.vue';

  export default{
    name: 'App',
    components: {
    Header,
    PrimeiroComponente,
    LifeCycle,
    Pessoa
},
    data(){
      return{
        testando: 'teste'
      }
    }
  }
</script>

<style>
  body{
    background-color: #333;
    color: white;
    margin: 0;
    padding: 0;
  }
  
  .componentes{
    padding: 30px;
  }

  a{
    color: yellow;
    text-decoration: none;
  }
</style>