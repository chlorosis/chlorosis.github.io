<script setup lang="ts">
import { ref } from 'vue';


const projects = ref([]);
</script>

<template>
  <section id="portfolio">
    <h1>My work so far</h1>
    <div class="container">
      <slot></slot>
    </div>

  </section>
</template>


<style scoped lang="sass">
.container
    display: flex 
    gap: 1rem
    flex-direction: column
    align-items: center
    width: 100%
    overflow: hidden


h1
  text-align: center
</style>
