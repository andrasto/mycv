<template>
    <div id="app">
        <app-header></app-header>
        <hr>
    </div>
</template>

<script>
    import appHeader from './components/Header.vue'

    export default {
        name: 'app',
        data () {
            return {
                msg: 'Welcome to Your Vue.js App'
            }
        },
        components: {
            appHeader
        }
    }
</script>

<style lang="scss">
    div#app {
        width: 50%;
        margin: auto;
    }

    section.indent {
        margin-left: 1rem;
    }
</style>
