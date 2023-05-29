<script>
    export default {
        name: 'diretivas-component',
        data() {
            return {
                working: true,
                button_text: "Demitir"
            }
        },
        methods: {
            workClick() {
                this.working = !this.working
                this.button_text = this.working?"Demitir":"Contratar"
            }
        }
    }
</script>
<template>
    <p v-if="this.working">Estou trabalhando!</p>
    <p v-else>Não estou trabalhando!</p>
    <button v-on:click="workClick">{{ button_text }}</button>
</template>