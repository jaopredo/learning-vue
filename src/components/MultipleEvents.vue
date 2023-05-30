<script>
    export default {
        name: 'multiple-events',
        data() {
            return {
                eventos_texto: ""
            }
        },
        methods: {
            first() {
                this.eventos_texto = "Alterado no primeiro evento"
            },
            second() {
                setTimeout(()=>this.eventos_texto="Alterado no segundo evento", 5000)
            }
        }
    }
</script>

<template>
    <p>Ativar os múltiplos eventos</p>
    <p>Texto: {{ eventos_texto }}</p>
    <button @click="first($event), second($event)">ATIVAR</button>
</template>