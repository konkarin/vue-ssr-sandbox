<script setup lang="ts">
import { ref } from "vue";

const count = ref(import.meta.env.SSR ? 0 : 1);
</script>

<template>
  <div>
    <button type="button" @click="count++">count is {{ count }}</button>
    <div>hello</div>
  </div>
</template>
