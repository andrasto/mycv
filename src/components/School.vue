<template>
    <div class="grid-container">
        <div class="grid-item">
            <b><p>{{ school.major }}</p></b>
            <p> - </p>
            <p>{{ school.place }}</p>
        </div>
        <div class="grid-item">
            <p>{{ school.timePeriod }}</p>
        </div>
    </div>
</template>

<script>
export default {
    props: ['school']
}
</script>

<style lang="scss" scoped>
    
</style>