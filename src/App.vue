<template>
    <div id="app">
        <Index/>
        <Slots>
            <template v-slot:paragraph>
                My slot paragraph
            </template>
            <template v-slot:header>
                My slot header
            </template>
            <template v-slot:span>
                My slot span
            </template>
        </Slots>

    </div>
</template>

<script>
    import Index from './components/Index.vue'
    import Slots from './components/Slots'

    export default {
        name: 'app',
        components: {
            Index,
            Slots
        }
    }
</script>

<style>
    #app {
        font-family: 'Avenir', Helvetica, Arial, sans-serif;
        -webkit-font-smoothing: antialiased;
        -moz-osx-font-smoothing: grayscale;
        /*text-align: center;*/
        color: #2c3e50;
        /*margin-top: 60px;*/
    }
</style>


