<template>
    <div>
        <h2>Está é a descrição da pessoa: {{ nome }}</h2>
    <p v-if="esta_trabalhando">Estou trabalhando no momento.</p>
    <p v-else>Estou em busca de uma oportunidade.</p>
    <p>Utilizo as seguintes tecnologias:</p>
    <ul>
        <li>HTML5</li>
        <li>CSS3</li>
        <li>Javascript</li>
        <li>JQuery</li>
        <li>Vue JS</li>
        <li>Bootstrap 5</li>
    </ul>
    <p v-show="mostrar_email">Mande uma mensagem para: {{ email }}</p>
    </div>
</template>

<script>
    export default{
        name: 'Info',
        data(){
            return{
            esta_trabalhando: true,
            mostrar_email: true,
            email: 'victor@gmail.com'
            }
        }
    }
</script>