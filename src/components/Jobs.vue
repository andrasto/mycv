<template>
    <div>
        <div class="grid-container">
            <div class="grid-item">
                <b><p>{{ job.title }}</p></b>
            </div>
            <div class="grid-item">
                <p>{{ job.timePeriod }}</p>
            </div>
        </div>
        <ul>
            <li v-for="description in job.description" 
                :key="description" 
                v-html="description"></li>
        </ul>
    </div>
</template>

<script>
export default {
    props: ['job']
}
</script>

<style lang="scss" scoped>
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