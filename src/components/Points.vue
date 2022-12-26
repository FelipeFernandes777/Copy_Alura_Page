<template>
  <div class="point">
    <div class="text">
      <p class="xp">
      21.1K
      <span class="color_xp">xp</span>
    </p>
    </div>
    <div class="points_container">
      <div class="points"></div>
      <div class="points"></div>
      <div class="points_activate" id="activate"></div>
      <div class="points"></div>
      <div class="points"></div>
      <div class="points"></div>
      <div class="points"></div>
      <div class="points"></div>
      <div class="points_activate" id="activate"></div>
      <div class="points"></div>
      <div class="points"></div>
      <div class="points"></div>
      <div class="points"></div>
      <div class="points"></div>
      <div class="points"></div>
      <div class="points"></div>
      <div class="points_activate" id="activate"></div>
      <div class="points_activate" id="activate"></div>
      <div class="points"></div>
      <div class="points"></div>
      <div class="points"></div>
      <div class="points"></div>
      <div class="points"></div>
      <div class="points"></div>
      <div class="points_activate" id="activate"></div>
      <div class="points"></div>
      <div class="points"></div>
      <div class="points"></div>
      <div class="points"></div>
      <div class="points_activate" id="activate"></div>
    </div>
  </div>
</template>

<script>
export default {
  name: "Points-Container"
}
</script>

<style scoped>

.text{
  display: flex;
  align-items: flex-end;
  justify-content: end;
}

.xp {
  font-weight: 400;
  font-size: 15px;
  color: #ffffff;
}

.color_xp {
  color: #169ec2;
}

.points_container {
  display: flex;
  justify-content: flex-end;
  align-items: flex-end;
  flex-wrap: wrap;
  background-color: #051932;
  width: 89px;
  padding: 4px;
}

.points {
  width: 6px;
  margin: 1px;
  height: 6px;
  background-color: #3d608f;
}

.points_activate {
  width: 6px;
  height: 6px;
  background-color:#169ec2;
  margin: 1px;
}

</style>
