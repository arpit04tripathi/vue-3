<template>
    <div>
        <h1>This is bootstrap view</h1>
        <TestBootstrapIcons />
    </div>
</template>

<script setup lang="ts">
import TestBootstrapIcons from '../components/test/TestBootstrapIcons.vue'
</script>

<style>
@media (min-width: 1024px) {
  .about {
    min-height: 100vh;
    display: flex;
    align-items: center;
  }
}
</style>
