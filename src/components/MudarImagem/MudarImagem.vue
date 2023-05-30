<template>
    <input type="file" @change="changePath" accept="image/png, image/jpeg">
    <button @click="$emit('mudar-imagem', file_path)">MUDAR IMAGEM</button>
</template>

<script>
export default {
    name: 'mudar-imagem',
    data() {
        return {
            file_path: ''
        }
    },
    methods: {
        changePath(e) {
            const { value } = e.target
            this.file_path = value
        }
    },
    emits: [ 'mudar-imagem' ]
}
</script>