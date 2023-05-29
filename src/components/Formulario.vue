<template>
    <form>
        <input type="text" v-model="input_name" placeholder="Digite seu nome">
    </form>
    <button v-on:click="submitForm">Enviar</button>
    <p>
        Seu nome é: {{ input_name }}
    </p>
</template>

<script>
    export default {
        name: "Formulario-biding",
        data() {
            return {
                input_name: "",
                teste: ""
            }
        },
        methods: {
            submitForm(e) {
                e.preventDefault()
            }
        }
    }
</script>