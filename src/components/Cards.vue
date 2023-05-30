<script>
    import Card from './Card/Card.vue'

    export default {
        name: 'items-list',
        data() {
            return {
                cardsInfos: [
                    {
                        id: 1,
                        title: "Título 1",
                        text: "Esse texto é um teste"
                    },
                    {
                        id: 2,
                        title: "Título 2",
                        text: "Esse texto é um teste"
                    }
                ]
            }
        },
        components: {
            Card
        }
    }
</script>

<template>
    <ul class="cardsList">
        <Card v-for="{ title, text, id } in cardsInfos" v-bind:key="id" :title="title" :text="text"/>
    </ul>
</template>

<style scoped>
    .cardsList {
        display: flex;
        flex-direction: row;
        gap: 10px;
        align-items: center;
        justify-content: center;
    }
</style>