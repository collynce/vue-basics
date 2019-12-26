<template>
    <div>
        <Data message="This is a prop" value/>
        <Data message="This is another prop" value/>
    </div>
</template>

<script>
    import Data from './Data'
    export default {
        name: "Props",
        components:{
            Data
        }
    }
</script>

<style scoped>
div{
    background: aquamarine;
    padding: 7px;
}
</style>
