<template>
  <div class="logo_container">
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
  </div>
</template>

<script>
export default {
  name: "logo-component",
};
</script>

<style scoped>
.logo_header {
  height: 80px;
  display: flex;
  align-items: center;
  justify-content: center;
}

.logo_alura_icon {
  align-self: center;
  width: 80px;
  height: 38px;
}

.search_container {
  width: 30px;
  height: 30px;
  margin-left: 42px;
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
