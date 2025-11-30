<script setup lang="ts">
import { ref } from "vue";
import type { Ref } from "vue";

const count: Ref<number> = ref(0);
</script>

<template>
  <div id="count">
    <div class="count-container">
      <span class="count">{{ count }}</span>
    </div>
    <button class="btn" @click="count++">Count</button>
  </div>
</template>

<style scoped>
.count-container {
  margin-bottom: 1rem;
}
.count {
  font-size: 24px;
}
.btn {
  background-color: black;
  color: white;
  border: 1px solid black;
  border-radius: 6px;
}
</style>
