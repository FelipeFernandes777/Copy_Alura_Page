<template>
  <div class="title_header">
    <h1>{{ title }}</h1>
  </div>
</template>

<script>
export default {
  name: "Title-Component",
  props: {
    title: {
      type: String,
      required: true,
    },
  },
};
</script>

<style scoped>
h1 {
  font-size: 20px;
  line-height: 12px;
  color: #FFFFFF;
  font-weight: 900;
}
</style>
