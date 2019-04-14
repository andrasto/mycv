<template>
    <div id="app">
        <app-header></app-header>
        <hr>
        <app-education></app-education>
        <hr>
        <app-technical-strengths></app-technical-strengths>
        <hr>
        <app-work-experience></app-work-experience>
        <hr>
        <app-language></app-language>
    </div>
</template>

<script>
import appHeader from './components/Header.vue'
import appEducation from './components/Education.vue'
import appTechnicalStrengths from './components/TechnicalStrengths.vue'
import appWorkExperience from './components/WorkExperience.vue'
import appLanguage from './components/Language.vue'

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
        appWorkExperience,
        appLanguage
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
                padding: 0.5rem 0;
                display: inline-block;
            }
        }
    }

    ul {
        margin: 0;
        padding-left: calc(1rem + 10px);
        list-style-type: none;

        li {
            margin: 0.5rem 0;
        }

        li:before {
            content: "-";
            position: absolute;
            margin-left: -10px;
        }
    }
</style>
