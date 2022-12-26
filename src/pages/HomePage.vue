<template>
  <div class="home_page_container">
    <header>
      <HeaderVue />
    </header>
    <main class="dashboard">
      <MainContentVue />
    </main>
    <footer>

    </footer>
  </div>
</template>

<script>

import HeaderVue from '@/templates/Header.vue';
import MainContentVue from '@/templates/MainContent.vue';

export default {
  name: "HomePage-Component",
  components: {
    HeaderVue,
    MainContentVue,
  }
}
</script>

<style>
.dashboard {
  width: 100%;
  display: flex;
  justify-content: center;
  flex-wrap: wrap;
}
</style>
