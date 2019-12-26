<template>
    <div>
        <Navbar/>
        <Navbar/>
        <Navbar/>
        <p>This is the main component</p>
        <Props></Props>
    </div>
</template>
<script>
    import Navbar from './Navbar'
    import Props from './Props'

    export default {
        name: "Index",
        components: {
            Navbar,
            Props
        }
    }
</script>

<style scoped>

</style>
