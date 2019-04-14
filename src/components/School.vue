<template>
    <div class="grid-container">
        <div class="grid-item">
            <b><slot name="major"></slot></b>
            <p> - </p>
            <slot name="place"></slot>
        </div>
        <div class="grid-item">
            <slot name="timePeriod"></slot>
        </div>
    </div>
</template>

<script>
export default {
}
</script>

<style lang="scss" scoped>
    
</style>