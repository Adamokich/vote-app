<script setup lang="ts">
import '../vote-app/assets/main.css'
</script>

<template>
  <div>
    <NuxtLayout>
      <NuxtPage />
    </NuxtLayout>
  </div>
</template>

<style scoped>
.page-enter-active,
.page-leave-active {
  transition: all .2s;
}

.page-enter-active-from,
.page-leave-to {
  opacity: 0;
}
</style>
