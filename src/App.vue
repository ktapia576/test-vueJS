<template>
  <img alt="Vue logo" src="./assets/logo.png" />
  <HelloWorld v-bind:msg="75+1" />
  <todoList greeting="HELLO"/>
</template>

<script>
import HelloWorld from './components/HelloWorld.vue';
import todoList from './components/todoList.vue';


export default {
  components: {
    HelloWorld,
    todoList
  }
}

// This starter template is using Vue 3 experimental <script setup> SFCs
// Check out https://github.com/vuejs/rfcs/blob/script-setup-2/active-rfcs/0000-script-setup.md
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