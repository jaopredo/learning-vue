<template>
    <img :src="url" alt="imagem">
    <MudarImagem @mudar-imagem="mudarImagem($event)" />
</template>

<script>
import MudarImagem from './MudarImagem/MudarImagem.vue'

export default {
    name: 'imagem-emit',
    components: { MudarImagem },
    data(){
        return {
            url: ''
        }
    },
    methods: {
        mudarImagem(new_path) {
            const filename = new_path.replace(/^.*[\\\/]/, '')
            this.url = `http://127.0.0.1:8081/${filename}`
        }
    }    
}
</script>