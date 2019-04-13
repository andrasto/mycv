<template>
    <div>
        <h2>Education</h2>
        <section class="indent">
            <app-school>
                <template v-slot:major>
                    <p><b>Computer engineering</b></p>
                </template>
                <template v-slot:place>
                    <p>Eötvös Loránd University, Budapest</p>
                </template>
                <template v-slot:time>
                    <p>2015 - </p>
                </template>
            </app-school>

            <app-school>
                <template v-slot:major>
                    <p><b>Computer engineering</b></p>
                </template>
                <template v-slot:place>
                    <p>University of Debrecen, Debrecen</p>
                </template>
                <template v-slot:time>
                    <p>2014 - 2015(1 semester)</p>
                </template>
            </app-school>

            <app-school>
                <template v-slot:major>
                    <p><b>Informatics</b></p>
                </template>
                <template v-slot:place>
                    <p>Neumann János Secondary School, Eger</p>
                </template>
                <template v-slot:time>
                    <p>2010 - 2014</p>
                </template>
            </app-school>
        </section>
    </div>
</template>

<script>
import appSchool from './School.vue'

export default {
    components: {
        appSchool
    }
}
</script>

<style scoped>
</style>