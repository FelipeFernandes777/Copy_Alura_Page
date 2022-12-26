<template>
  <div class="navigate_container">
    <nav class="row">
      <ul class="row">
        <li class="row">
          <a class="font_navigate" href="#"
            >MEU APRENDIZADO
            <img class="icon_navigate_down" src="../assets/svg/down.svg" />
          </a>
        </li>
        <li>
          <a class="font_navigate" href="#"
            >CONTEÚDO
            <img class="icon_navigate_down" src="../assets/svg/down.svg" />
          </a>
        </li>
        <li>
          <a class="font_navigate" href="#"
            >COMUNIDADE
            <img class="icon_navigate_down" src="../assets/svg/down.svg" />
          </a>
        </li>
      </ul>
      <img
        src="../assets/svg/notifications.svg"
        alt="Bell"
        class="notification"
      />
      <div class="personal_section">
        <div class="points_container_person">
          <PointsVue />
        </div>
      </div>
    </nav>
  </div>
</template>

<script>
import PointsVue from "./Points.vue";

export default {
  name: "Navigate-Component",
  components: {
    PointsVue,
  },
};
</script>

<style scoped>
.navigate_container {
  display: flex;
  flex-direction: row;
  flex-wrap: nowrap;
  align-items: center;
  justify-content: space-between;
  height: 80px;
  width: auto !important;
  padding: 7px;
}

nav {
  display: flex;
  height: 100%;
}

ul {
  padding: 5px;
  list-style: none;
  display: flex;
  align-items: center;
  flex-direction: row;
}

li {
  margin: 5px;
}

.font_navigate {
  display: flex;
  align-items: center;
  justify-content: center;
  text-decoration: none;
  margin-left: 12px;
  color: #fff;
  font-size: 15px;
  font-weight: light;
}

.icon_navigate_down {
  width: 22px;
  margin-left: 8px;
  height: 22px;
}

.notification {
  margin: 12px;
  widows: 45px;
  height: 45px;
}
</style>
