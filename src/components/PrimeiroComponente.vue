<template>
    <div>
    <h1>Olá Vue</h1>
    <p>Meu nome é {{ nome }}</p>
    <p>Eu trabalho como {{ profissao }}</p>
    <MultiplosEventos />
    </div>
</template>

<script>

    import MultiplosEventos from './MultiplosEventos.vue'

    export default {
        name: 'primeiroComponente',
        components: {
            MultiplosEventos
        },
        data(){
            return{
                nome: 'Victor',
                profissao: 'Desenvolvedor Front-end'

            }
        }
    }
</script>