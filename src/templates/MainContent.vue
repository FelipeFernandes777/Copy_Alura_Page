<template>
  <div class="main_content_container">
    <main class="flex">
      <div class="progess_courses_ongoing">
        <CourseOngoing />
      </div>
      <div class="progress_courses">
        <ProgressVue />
      </div>
    </main>
  </div>
</template>

<script>
import CourseOngoing from "@/components/CourseOngoing.vue";
import ProgressVue from "@/components/Progress.vue";

export default {
  name: "Main-Content-Component",
  components: {
    CourseOngoing,
    ProgressVue,
  },
};
</script>

<style scoped>
.flex {
  display: flex;
}
</style>
