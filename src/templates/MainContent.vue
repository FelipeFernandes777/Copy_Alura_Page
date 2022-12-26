<template>
  <div class="main_content_container">
    <main>
      <div class="progess_courses">
        <ProgressVue />
      </div>
    </main>
  </div>
</template>

<script>

import ProgressVue from '@/components/Progress.vue';

export default {
  name: 'Main-Content-Component',
  components: {
    ProgressVue
  }
}
</script>

<style scoped>
</style>
