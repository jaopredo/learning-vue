<script>
    export default {
        name: 'Life-Cycle',
        data() {
            return {
                nome: "sei la"
            }
        },
        created() {
            this.nome = "Alterado"
        }
    }
</script>

<template>
    <p>Meu nome é {{ nome }}</p>
</template>