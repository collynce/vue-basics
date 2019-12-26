<template>
    <div>
        <p></p>
        <button v-on:click="myAlert">Data</button>
    </div>
</template>

<script>
    export default {
        name: "ChildComponent",
        data() {
            return {
                // changeColor: 'red'
            }
        },
        methods: {
            myAlert() {
                this.$emit('show-alert');
            }
        }
    }
</script>

<style scoped>

</style>

