<template>
    <div>
        <slot/>
    </div>
</template>

<script>
    export default {
        name: "Blue"
    }
</script>

<style scoped>
    div {
        border: 1px solid blue;
        background-color: lightblue;
        padding: 30px;
        margin: 20px auto;
        text-align: center
    }
</style>
