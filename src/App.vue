<template>
    <div id="app">
        <app-header></app-header>
        <hr>
        <app-education></app-education>
        <hr>
        <app-technical-strengths></app-technical-strengths>
        <hr>
        <app-work-experience></app-work-experience>
    </div>
</template>

<script>
import appHeader from './components/Header.vue'
import appEducation from './components/Education.vue'
import appTechnicalStrengths from './components/TechnicalStrengths.vue'
import appWorkExperience from './components/WorkExperience.vue'

export default {
    name: 'app',
    data () {
        return {
            
        }
    },
    components: {
        appHeader,
        appEducation,
        appTechnicalStrengths,
        appWorkExperience
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

    .grid-container {
        display: grid;
        grid-template-columns: 70% 30%;

        .grid-item {
            p {
                margin: 0;
                display: inline-block;
            }
        }
    }
</style>
