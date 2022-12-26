<template>
  <div class="header_component_conteiner">
    <div class="header_main_container">
      <div class="content">
        <div class="logo_header">
          <img
            src="../assets/svg/logo-alura.svg"
            alt="Logo Alura"
            class="logo_alura_icon"
          />
          <div class="search_container">
            <img
              src="../assets/svg/icons8-search.svg"
              alt="search"
              class="search"
            />
          </div>
        </div>
        <div class="navigation_header_container">
          <NavigateVue />
        </div>
      </div>
    </div>
    <section class="sub_header_component_container">
      <TitleHeaderVue title="DASHBOARD" />
    </section>
  </div>
</template>

<script>
import NavigateVue from "@/components/Navigate.vue";
import TitleHeaderVue from "@/components/TitleHeader.vue";

export default {
  name: "Header-Component",
  components: {
    TitleHeaderVue,
    NavigateVue,
  },
};
</script>

<style scoped>
:root {
  --line-color-blue: #2a7ae4;
  --bg-header-color: #051932;
  --bg-sub-header-color: #093364;
}

.header_main_container {
  width: 100%;
  height: 80px;
  display: flex;
  align-items: center;
  flex-wrap: wrap;
  flex-direction: row;
  background-color: #051932;
  border-top: 4px solid #2a7ae4;

  justify-content: center;
}

.content {
  align-items: center;
  justify-content: space-between;
  display: flex;
  width: 60%;
}

.navigation_header_container {
  display: flex;
  flex-direction: row;
}

.logo_header {
  height: 80px;
  display: flex;
  align-items: center;
  justify-content: center;
}

.logo_alura_icon {
  align-self: center;
  width: 80px;
  height: 36px;
}

.search_container {
  width: 30px;
  height: 30px;
  margin-left: 25px;
  border-radius: 4px;
  background-color: #2a7ae4;

  display: flex;
  align-items: center;
  justify-content: center;
  align-self: flex-start;
}

.search {
  width: 19px;
  height: 19px;
}
</style>
