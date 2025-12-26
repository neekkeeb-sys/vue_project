<script setup>
import { ref } from 'vue'

const blogs = ref([
  { id: 1, title: 'Vue 3 Basics', content: 'Vue is awesome' },
  { id: 2, title: 'Vue Router', content: 'Routing in Vue 3' },
  { id: 3, title: 'Vue with Django', content: 'Frontend + Backend' }
])
</script>

<template>
  <div>
    <h1>My Blog</h1>

    <ul>
      <li v-for="blog in blogs" :key="blog.id">
        <RouterLink :to="`/blog/${blog.id}`">
          {{ blog.title }}
        </RouterLink>
      </li>
    </ul>
  </div>
</template>
