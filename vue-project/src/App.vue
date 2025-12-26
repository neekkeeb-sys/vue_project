<script setup>
import { RouterView, RouterLink } from 'vue-router'
</script>

<template>
  <div>
    <nav style="margin-bottom: 20px">
      <RouterLink to="/">Home</RouterLink>
    </nav>

    <RouterView />
  </div>
</template>
