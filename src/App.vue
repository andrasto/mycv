<template>
    <div id="app">
        <app-header></app-header>
        <hr>
        <app-education></app-education>
        <hr>
        <app-technical-strengths></app-technical-strengths>
    </div>
</template>

<script>
import appHeader from './components/Header.vue'
import appEducation from './components/Education.vue'
import appTechnicalStrengths from './components/TechnicalStrengths.vue'

export default {
    name: 'app',
    data () {
        return {
            
        }
    },
    components: {
        appHeader,
        appEducation,
        appTechnicalStrengths
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

    h2 {
        color: #78a6cf;
    }
</style>
