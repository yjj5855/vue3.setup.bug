<script setup>
import {ref, reactive} from 'vue'
const ref_form = ref(null)
const form = reactive({name: '', password: ''})
</script>

<script>
export default {
  mounted() {
    console.log(this.ref_form)
    console.log(this.form)
  }
}
</script>

<template>
  <img ref="ref_form" alt="Vue logo" src="./assets/logo.png" />
</template>

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
