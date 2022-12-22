<template>
    <div>
    <h1>Olá Vue</h1>
    <p>Meu nome é {{ nome }}</p>
    <p>Eu trabalho como {{ profissao }}</p>
    </div>
</template>

<script>
    export default {
        name: 'primeiroComponente',
        data(){
            return{
                nome: 'Victor',
                profissao: 'Desenvolvedor Front-end'

            }
        }
    }
</script>