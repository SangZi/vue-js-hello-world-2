<template>
  <img alt="Vue logo" src="./assets/logo.png">
  <HelloWorld msg="Welcome to Your Vue.js App"/>
  <MyFirstComponent></MyFirstComponent>
  <MySecondComponentForContact></MySecondComponentForContact>
  <my-button></my-button>
</template>

<script>
import HelloWorld from './components/HelloWorld.vue'
import MyFirstComponent from "@/components/MyFirstComponent.vue";
import MySecondComponentForContact from "@/components/MySecondComponent.vue";
import MyButton from "@/components/MyButton.vue";

export default {
  name: 'App',
  components: {
    HelloWorld,
    MyFirstComponent,
    MySecondComponentForContact,
    MyButton
  }
}
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
