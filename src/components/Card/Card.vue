<script>
    export default {
        name: 'card-item',
        props: [ 'title', 'text' ]
    }
</script>

<template>
    <li class="cardItem">
        <h2>{{ title }}</h2>
        <p>{{ text }}</p>
    </li>
</template>

<style scoped>
    .cardItem {
        border: 1px solid #0cff7e;
        background: #0e0e0e;
        border-radius: 5px;
        color: white;
        padding: 10px;
        list-style: none;
    }
    h2 {
        color: #0cff7e;
    }
</style>
