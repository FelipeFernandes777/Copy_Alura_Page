<template>
  <div class="header_component_conteiner">
    <div class="header_main_container">
      <div class="content">
        <LogoVue />        
        <div class="navigation_header_container">
          <NavigateVue />
        </div>
      </div>
    </div>
    <section class="sub_header_component_container">
      <div class="text_sub_header_container">
        <TitleHeaderVue title="DASHBOARD" class="text_sub_header"/>
      </div>
    </section>
  </div>
</template>

<script>
import LogoVue from "@/components/Logo.vue";
import NavigateVue from "@/components/Navigate.vue";
import TitleHeaderVue from "@/components/TitleHeader.vue";

export default {
  name: "Header-Component",
  components: {
    TitleHeaderVue,
    NavigateVue,
    LogoVue,
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
  width: 63%;
}

.navigation_header_container {
  display: flex;
  flex-direction: row;
}

.sub_header_component_container {
  width: 100%;
  height: 70px;
  display: flex;
  align-items: center;
  justify-content: center;
  background-color: #093364;
}

.text_sub_header_container {
  width: 63%;
}
</style>
