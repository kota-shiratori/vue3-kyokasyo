<script setup lang="ts">
import { ref } from 'vue';

const imgAttributes = ref({
  src: "/images/src/assets/logo.svg",
  alt: "Vue logo",
  width: 75,
  height: 75
});
</script>

<template>
  <p>
    <img v-bind="imgAttributes">
  </p>
  <p>
    <img v-bind="imgAttributes" title="ロゴです！">
  </p>
  <p>
    <img v-bind="imgAttributes" alt="ロゴです！">
  </p>
</template>