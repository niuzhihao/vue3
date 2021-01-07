<template>
  <div class="about">
    <h1>This is an about page {{ count }}</h1>
    <button @click="changeCount">+</button>
  </div>
</template>

<script>
import { ref } from "vue";
export default {
  setup(props, context) {
    const count = ref(0)

    const changeCount = () => {
      count.value++
    }

    return { count, changeCount }
  }
}
</script>
