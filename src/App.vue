<template>
  <div>
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
  
  
</template>

<script>

  import PrimeiroComponente from './components/PrimeiroComponente.vue';
  import LifeCycle from './components/LifeCycle.vue';
  import Pessoa from './components/Pessoa.vue';

  export default{
    name: 'App',
    components: {
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