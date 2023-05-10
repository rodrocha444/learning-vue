<script setup lang="ts">
  const props = defineProps({
    textOfAd: String
  })
</script>

<template>
  <div id="ad">{{ props.textOfAd }}</div>
</template>

<style>
  #ad{
    text-align: center;
    width: 100%;
    padding: 0.8rem;

    color: #424242;
    background-color: white;
    font-size: 0.95rem;
  }
</style>