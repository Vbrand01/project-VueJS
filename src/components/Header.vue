<template>
    <ul>
        <li><a href="">Home</a> </li>
        <li><a href="">Serviços</a></li>
        <li><a href="">Contatos</a></li>
    </ul>
</template>

<script>
    export default{
        name: 'Header'
    }
</script>

<style scoped>

    ul{
        list-style: none;
        display: flex;
        background-color: rgb(65, 65, 65);
        padding: 15px;
        border-radius: 10px;
        margin-top: 0;
    }

    li{
        margin-right: 10px;
    }
    
    a{
        color: white;
        text-decoration: none;
        transition:  .5s;
    }

    a:hover{
        color: turquoise;
    }

</style>