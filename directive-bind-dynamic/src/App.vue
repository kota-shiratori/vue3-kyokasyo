<script setup lang="ts">
import { ref } from 'vue';

const widthOrHeight = ref("height");

const widthOrHeightValue = ref(600);
</script>

<template>
  <p>
    <img src="./assets/logo.svg" v-bind:[widthOrHeight]="widthOrHeightValue" />
  </p>
</template>