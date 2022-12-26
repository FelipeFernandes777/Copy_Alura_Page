<template>
  <div class="person_container_navigate">
    <div class="person_image">
      <a href="#">
        <img
          src="../assets/img/images.jpeg"
          alt="Icon Person Photo"
          class="person"
        />
        <span class="text_person">EMANUELLE</span>
        <span
          ><img
            src="../assets/svg/down.svg"
            alt="Down Arrow"
            class="down_arrow"
        /></span>
      </a>
    </div>
  </div>
</template>

<script>
export default {
  name: "Person-component",
};
</script>

<style scoped>
.person_image a {
  display: flex;
  align-items: center;
  justify-content: center;
  text-decoration: none;
}

.person {
  width: 45.7px;
  height: 45.7px;
  border-radius: 50%;
  margin: 0px 20px 0px 13px;
}

.text_person {
  color: #ffffff;
  font-size: 14px;
  font-weight: 600;
  margin: 0px 12px 0px 0px;
}

.down_arrow {
  width: 12px;
  height: 12px;
}
</style>
