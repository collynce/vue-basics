<template>
    <div>
        <p>{{message}}</p>
        <slot></slot>
    </div>
</template>

<script>

    export default {
        name: "Data",
        props: {
            message: String
        }
    }
</script>

<style scoped>

</style>
