<template>
  <div class="container">
    <h1>hello</h1>
    <div class="count">
      <span>count is {{ count }}</span>
      <button @click="count++">+1</button>
    </div>
  </div>
</template>

<script>
import { ref } from 'vue';
export default {
  setup() {
    const count = ref(6);
    function add() {
      count.value ++;
    }
    return { count, add };
  }
}
</script>
