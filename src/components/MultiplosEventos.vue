<template>

    <div>

        <button @click="primeiro(txt1, $event), segundo(txt2,$event), terceiro(txt3, $event)">Ativar múltiplos eventos</button>
        <p>{{ multiplos_eventos }}</p>

    </div>

</template>

<script>

    export default {
        name: 'MultilplosEventos',

        data(){
            return {
                multiplos_eventos: "",
                txt1: "Primeiro evento",
                txt2: "Segundo evento",
                txt3: "Terceiro evento"
            }

        },

        methods: {
            primeiro(txt, e){
                this.multiplos_eventos = txt;
            },
            segundo(txt, e){
                setTimeout(()=> {
                    this.multiplos_eventos = txt;
                }, 700)
            },
            terceiro(txt, e){
                setTimeout(()=> {
                    this.multiplos_eventos = "";
                }, 1400)
            }
        }
    }

</script>

<style scoped>
div{
    margin: 100px;
}

</style>