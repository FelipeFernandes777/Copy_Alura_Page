<template>
  <div class="in_courses">
    <div class="container">
      <div class="title_container">
        <h2 class="title_course">Meus cursos em andamento</h2>
      </div>
      <section class="ongoing_courses">
        <div class="main_course_ongoing">
          <CourseMainVue
            progess_percentage="66%"
            pictureSrc="svg/projetos-de-algoritmos-1.svg"
            pictureAlt="Algoritmos Logo"
            titleCourse="Algoritmos I: Selection, Insertion"
            descriptionBold="Aula atual: "
            description="Representando os produtos - 20min"
          />
        </div>
        <div class="column_course_ongoing">
          <CourseVue
            pictureSrc="svg/vue3-comecando-framework.svg"
            pictureAlt="Vue3_Logo"
            titleCourse="CURSO"
            description="Vue3: explorando o framework"
            progess_percentage="50%"
          />
          <AgilVue
            pictureSrc="svg/fundamentos-agilidade.svg"
            pictureAlt="Agile_Logo"
            titleCourse="CURSO"
            description="Agilidade: promovendo a transformação ágil"
            progess_percentage="88%"
          />
        </div>
      </section>
    </div>
  </div>
</template>

<script>
import AgilVue from "./Agil.vue";
import CourseVue from "./Course.vue";
import CourseMainVue from "./CourseMain.vue";

export default {
  name: "Progress-Courses-Container",
  components: {
    CourseMainVue,
    CourseVue,
    AgilVue,
  },
};
</script>

<style scoped>
.main_course_ongoing {
  width: 50%;
}

.in_courses {
  width: 600px;
  height: 660.91px;
}

.title_course {
  color: #74849d;
  font-size: 22px;
}
</style>
