<script setup>
import { useRoute } from 'vue-router'

const route = useRoute()
</script>

<template>
  <div>
    <h2>Blog ID: {{ route.params.id }}</h2>
    <RouterLink to="/">⬅ Back</RouterLink>
  </div>
</template>
