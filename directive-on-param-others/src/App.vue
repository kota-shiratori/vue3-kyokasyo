<script setup lang="ts">
import { ref } from 'vue';

const pBgcolor = ref("white");
const onPClick = (bgColor: string): void => {
  pBgcolor.value = bgColor;
};
</script>

<template>
  <p v-on:click="onPClick('red')" v-bind:style="{ backgroundColor: pBgcolor }">ここをクリックすると背景色が変わります。</p>
</template>
