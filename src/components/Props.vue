<script>
    export default {
        name: 'Components-Props',
        props: [ 'prop1', 'prop2' ]
    }
</script>

<template>
    <p>Valor da Propriedade 1: {{ prop1 }}</p>
    <p>Valor da Propriedade 2: {{ prop2 }}</p>
</template>