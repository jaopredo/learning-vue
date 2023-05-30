<template>
    <div id="toStyle">
        Esse componente está estilizado localmente!
    </div>
</template>

<script>
    export default {
        name: 'scoped-style',
    }
</script>

<style scoped>
    #toStyle {
        background: #c9c9c9;
        color: black;
        padding: 20px;
        border-radius: 5px;
        box-shadow: 3px 3px 10px black;
        text-align: center;
        width: 60%;
        margin: auto;
        margin-bottom: 20px;
    }
</style>