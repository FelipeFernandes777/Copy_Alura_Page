<template>
  <div class="navigate_container">
    <nav>
      <ul>
        <li>
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
      <div class="points_container_person">
        <PointsVue />
      </div>
      <div class="person_section">
        <PersonVue />
      </div>
    </nav>
  </div>
</template>

<script>
import PersonVue from "./Person.vue";
import PointsVue from "./Points.vue";

export default {
  name: "Navigate-Component",
  components: {
    PointsVue,
    PersonVue,
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
  padding: 11px;
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
  font-size: 14px;
  font-weight: 600;
}

.icon_navigate_down {
  width: 10px;
  margin-left: 8px;
  height: 10px;
}

.notification {
  margin: 12px 25px 12px 12px;
  width: 26px;
  height: 26px;
}

.person_section {
  display: flex;
  flex-direction: row;
  align-items: center;
  justify-content: center;
}
</style>
