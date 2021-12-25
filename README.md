# bug 代码在App.vue中
如下
```
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

```