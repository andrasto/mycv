<template>
    <div class="grid-container">
        <div class="grid-item">
            <slot name="major"></slot>
            <p> - </p>
            <slot name="place"></slot>
        </div>
        <div class="grid-item">
            <slot name="time"></slot>
        </div>
    </div>
</template>

<script>
export default {
}
</script>

<style lang="scss" scoped>
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