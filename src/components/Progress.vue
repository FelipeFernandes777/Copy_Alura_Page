<template>
  <div class="progress_card">
    <div class="title_container">
      <h2 class="title_course">Progresso em Formação</h2>
    </div>
    <div class="progress_card_container"></div>
  </div>
</template>

<script>
export default {
  name: "Progress-Container-Component",
  components: {},
};
</script>

<style scoped>
.progress_card {
  margin-left: 30px;
}
.progress_card_container {
  width: 600px;
  border: 1px solid black;
  height: 420px;
}

.title_course {
  color: #74849d;
  font-size: 22px;
  margin-bottom: 18px;
}
</style>
