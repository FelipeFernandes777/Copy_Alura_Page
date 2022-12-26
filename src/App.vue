<template>
  <div id="app">
    <HomePageVue />
  </div>
</template>

<script>
import HomePageVue from "./pages/HomePage.vue";

export default {
  name: "App",
  components: {
    HomePageVue,
  },
};
</script>

<style>
* {
  padding: 0;
  margin: 0;
  box-sizing: border-box;
  font-family: "Open Sans", sans-serif;
}
</style>
