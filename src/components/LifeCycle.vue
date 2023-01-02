<template>
        <h1>Meu nome é: {{ nome }}</h1>
</template>

<script>
    export default{
        name: 'LifeCycle',
        data(){
            return{
                nome: '...'
            }
        },
        created(){
            setTimeout(()=> {
                this.nome = 'Matheus'
            }, 1000)
        },
        mounted(){
            setTimeout(()=> {
                this.nome = 'Victor'
            }, 3000)
        }
    }
</script>