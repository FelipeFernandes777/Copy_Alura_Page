<template>
  <div class="course_main_container_ongoing">
    <div class="progress">
      <div class="bar_progress">
        <div class="bar_progess_color"></div>
      </div>
      <p class="progress_percentage">{{ progess_percentage }}</p>
    </div>
    <div class="logo_course_main_ongoing">
      <img
        :src="require('@/assets/' + pictureSrc + '')"
        :alt="pictureAlt"
        class="icon_courses_ongoing"
      />
      <span class="title_course_main">{{ titleCourse }}</span>
    </div>
    <div class="description_course_main_ongoing">
      <span class="description_course_main_ongoing_bold">{{
        descriptionBold
      }}</span
      >{{ description }}
    </div>
    <div class="footer_main_course_ongoing">
      <div class="start_course"><a href="#">Continuar onde parou</a></div>
      <a href="#" class="forum">Fórum do curso</a>
    </div>
  </div>
</template>

<script>
export default {
  name: "Course-Component",
  props: {
    description: {
      type: String,
      required: true,
    },
    descriptionBold: {
      type: String,
      required: true,
    },
    titleCourse: {
      type: String,
      required: true,
    },
    pictureSrc: {
      type: String,
      required: true,
    },
    pictureAlt: {
      type: String,
      required: true,
    },
    progess_percentage: {
      type: String,
      required: true,
    },
  },
};
</script>

<style scoped>
.course_main_container_ongoing {
  width: 600px;
  height: 235px;
  border: 1px solid #eff1f9;
  margin-bottom: 35px;
  display: flex;
  flex-direction: column;
}

.progress {
  display: flex;
  align-items: center;
  flex-direction: row;
  flex-wrap: wrap;
  gap: 10px;
}

.bar_progress {
  height: 4px;
  width: 95%;
  background-color: #d7dbdf;
  display: flex;
}

.bar_progess_color {
  height: 4px;
  width: 66%;
  background-color: #5dda7b;
}

.progress_percentage {
  color: #8487b1;
  line-height: 9px;
  font-size: 10px;
}
.logo_course_main_ongoing {
  padding: 15px;
  display: flex;
  align-items: center;
}

.icon_courses_ongoing {
  margin: 0px 7px 0px 0px;
  width: 54px;
  height: 54px;
}

.title_course_main {
  color: #8487b1;
  font-size: 16px;
  font-weight: 400;
  line-height: 10px;
  padding: 12px;
}

.description_course_main_ongoing_bold {
  color: #525c65;
  font-size: 13.33px;
  font-weight: 700;
  margin-left: 15px;
}

.description_course_main_ongoing {
  font-size: 13.33px;
  color: #576183;
  line-height: 23px;
}

.footer_main_course_ongoing {
  margin: 12px;
  width: 100%;
  display: flex;
  align-items: center;
  justify-content: flex-start;
}

.start_course {
  padding: 10px 30px;
  background-color: #2087ed;
  width: auto;
  border-radius: 4px;
  margin-right: 24px;
  display: flex;
  align-items: center;
  justify-content: center;
  text-decoration: none;
}

.start_course a {
  color: white;
  text-decoration: none;
}

.forum {
  color: #525c65;
  font-size: 16px;
}
</style>
