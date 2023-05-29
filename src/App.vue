<script>
    import Componente from "./components/Componente.vue"
    import Formulario from './components/Formulario.vue'
    import LifeCycle from './components/LifeCycle.vue'
    import Props from './components/Props.vue'
    import Children from './components/Children.vue'
    import Diretivas from './components/Diretivas.vue'
    import Picture from './components/Picture.vue'
    export default {
        name: 'App',
        components: {
            Componente,
            Formulario,
            LifeCycle,
            Props,
            Children,
            Diretivas,
            Picture
        }
    }
</script>

<template>
    <h1>COMPONENTE BÁSICO</h1>
    <Componente/>
    
    <h1>DATA BIDING</h1>
    <p>Data biding é quando conseguimos alterar os valores das variáveis de um componente através dos inputs</p>
    <Formulario/>
    
    <h1>Life Cycle Hooks</h1>
    <p>São eventos que podem ser disparados em momentos específicos do código, como <strong>quando o componente é criado</strong></p>
    <LifeCycle/>

    <h1>Propriedades no componente e Passando Children</h1>
    <Props :prop1="'teste1'" :prop2="'teste2'"/>
    <Children>
        <p>Isso é um texto dentro >:O</p>
        <p>Componente dentro de outro:</p>
        <Props :prop1="'teste dentro 1'" :prop2="'teste dentro 2'"/>
    </Children>

    <h1>Diretivas</h1>
    <p>São eventos que podem ser colocados nos componentes que os tornam dinâmicos, como exibir vários itens de uma lista ou mostrar somente se uma <strong>condição</strong> for atendida</p>
    <ul>
        <li><strong>v-bind:href=""</strong> - Essa diretiva altera dinamicamente links que eu queira colocar como um valor de data</li>'
        <li><strong>v-if="" e v-else</strong> - Mostra um componente apenas se uma condição for atendida</li>
        <li><strong>v-show=""</strong> - Apenas diz se deve mostrar ou não o elemento</li>
    </ul>
    <Diretivas/>

    <h1>Atributos Dinâmicos</h1>
    <p>Alguns atributos de tags específicas que permitem uma melhor dinamização da aplicação, como a tag <strong>src</strong> de uma <strong>img</strong></p>
    <Picture/>
</template>

<style>
    *, *::after, *::before {
        padding: 0;
        margin: 0;
        border: none;
        box-sizing: border-box;
    }

    h1 {
        margin-top: 30px;
    }

    body {
        background-color: #1d1d1d;
        color: white;
        font-family: Arial, Helvetica, sans-serif;
    }
</style>