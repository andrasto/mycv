<template>
    <div>
        <h2>Education</h2>
        <section class="indent">
            <app-school v-for="(school, index) in schools" 
                        :key="index" 
                        :school="school">
            </app-school>
        </section>
    </div>
</template>

<script>
import appSchool from './School.vue'

export default {
    data() {
        return {
            schools: [
                {
                    major: 'Computer engineering',
                    place: 'Eötvös Loránd University, Budapest',
                    timePeriod: '2015 - '
                },
                {
                    major: 'Computer engineering',
                    place: 'University of Debrecen, Debrecen',
                    timePeriod: '2014 - 2015 (1 semester)'
                },
                {
                    major: 'Informatics',
                    place: 'Neumann János Secondary School, Eger',
                    timePeriod: '2010 - 2014'
                },
            ]
        }
    },
    components: {
        appSchool
    }
}
</script>

<style scoped>
</style>