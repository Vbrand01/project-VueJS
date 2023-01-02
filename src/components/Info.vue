<template>
    <div>
        <h2>Está é a descrição da pessoa: {{ nome }}</h2>
    <p v-if="esta_trabalhando">Estou trabalhando no momento.</p>
    <p v-else>Estou em busca de uma oportunidade.</p>
    <p>Utilizo as seguintes tecnologias para front-end:</p>
    <ul>
        <li v-for="(technology, index) in frontend_tec" v-bind:key="index">{{ technology }}</li>
    </ul>
    <p>Utilizo as seguintes tecnologias para front-end:</p>
    <ul>
        <li v-for="technology in backend_tec" :key="technology.id">
            {{ technology.language }}</li>
    </ul>
    <div>
        <button @click="showEmail">{{ textoBtn }}</button>
    </div>
    <p v-show="mostrar_email">Mande uma mensagem para: {{ email }}</p>
    <p>Para acessar meu portfólio <a v-bind:href="link_portfolio" target="_blank">Basta clicar aqui</a></p>

    <Picture />
    </div>
</template>

<script>

    import Picture from './Picture.vue' 

    export default{
        name: 'Info',
        components: {
            Picture
        },
        props: {
            email: String
        },
        data(){
            return{
            esta_trabalhando: true,
            mostrar_email: false,
            link_portfolio: 'https://vmbrandao.com/',
            textoBtn: 'Botão',
            frontend_tec: ['HTML5', 'CSS3', 'Javascript', 'JQuery', 'Vue JS', 'Bootstrap 5'],
            backend_tec: [
                {id: 1, language: 'PHP'},
                {id: 2, language: 'C#'},
                {id: 3, language: 'Node JS'}
            ]
            }
        },
        methods: {
            showEmail(){
                this.mostrar_email = !this.mostrar_email
                if(!this.mostrar_email){
                    this.textoBtn = 'Botão'
                } else {
                    this.textoBtn = 'Esconder'
                }
            }
        }
    }
</script>