<template>
    <div id="app">
        <app-header></app-header>
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

<style lang="scss" scoped>
    div#app {
        width: 50%;
        margin: auto;
    }
</style>
