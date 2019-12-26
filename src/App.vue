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
      <ChildComponent @show-alert="myAlert"></ChildComponent>
    </div>
</template>

<script>
    import Index from './components/Index.vue'
    import Slots from './components/Slots'
    import ChildComponent from "./components/ChildComponent";
    export default {
        name: 'app',
        components: {
            Index,
            Slots,
            ChildComponent
        },
      data(){
        return{
          Color: {
            background:'red'
          }
        }
      },
      methods:{
          myAlert(){
            alert('This is an event from the child component')
          }
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


