<template>
    <!-- <p>Estou trabalhando no momento.</p>
    <p>Utilizo as seguintes tecnologias:</p>
    <ul>
        <li>HTML5</li>
        <li>CSS3</li>
        <li>Javascript</li>
        <li>JQuery</li>
        <li>Vue JS</li>
        <li>Bootstrap 5</li>
    </ul> -->
    <Info />
    <Form />
</template>

<script>

    import Info from './Info.vue'
    import Form from './Form.vue'

    export default {
        name: 'Pessoa',
        components: {
            Info,
            Form
        },

        dados(){
            return{
                nome: 'Victor',
                sobrenome: 'Brandão',
                idade: 19,
                cidade: 'São Paulo',
                estado: 'SP'
            }
        }
    }

</script>