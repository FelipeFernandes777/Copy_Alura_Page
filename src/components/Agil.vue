<template>
  <div class="course_container_ongoing">
    <div class="logo_course">
      <img
        :src="require('@/assets/' + pictureSrc + '')"
        :alt="pictureAlt"
        class="icon_courses_ongoing"
      />
      <div class="description_card_courses_ongoing">
        <span class="title_course_ongoing">{{ titleCourse }}</span>
        <p class="description_course_ongoing">{{ description }}</p>
      </div>
    </div>
    <div class="progess">
      <div class="bar_progress">
        <div class="bar_progess_color"></div>
      </div>
      <p class="progess_percentage">{{ progess_percentage }}</p>
    </div>
  </div>
</template>

<script>
export default {
  name: "Course-Component",
  data() {
    return {};
  },
  props: {
    description: {
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
.course_container_ongoing {
  display: flex;
  align-items: center;
  justify-content: space-between;
  height: 70px;
  padding: 10px 0;

  border-left: 4px solid #a475ef !important;
  border: 1px solid rgba(0, 0, 0, 0.2);
}

.logo_course {
  display: flex;
  justify-content: center;
  flex-wrap: wrap;
  align-items: center;
}

.icon_courses_ongoing {
  margin: 0px 7px 0px 12px;
  width: 45px;
  height: 45px;
}

.description_card_courses_ongoing {
  display: flex;
  align-items: center;
  justify-content: flex-start;
  flex-direction: column;
}

.title_course_ongoing {
  font-size: 12px;
  color: #576183;
  line-height: 23px;
  font-weight: bold;
  align-self: flex-start;
}

.description_course_ongoing {
  color: #8487b1;
  line-height: 10px;
  font-size: 12px;
}

.progess {
  display: flex;
  align-items: center;
  justify-content: center;
  flex-wrap: wrap;
  gap: 10px;
}

.bar_progress {
  height: 4px;
  width: 100px;
  background-color: #d7dbdf;
}

.bar_progess_color {
  height: 4px;
  width: 88px;
  background-color: #5dda7b;
}

.progess_percentage {
  color: #8487b1;
  line-height: 9px;
  font-size: 10px;
}
</style>
