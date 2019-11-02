<template>
  <div>
    <div class="header">
      <h1>My Blog</h1>
    </div>
  </div>
</template>

<script>
export default {
  name: "Header",
  props: []
};
</script>

<style scoped>
h1 {
  color: white;
  background-image: url("../assets/beach.jpg");
  background-position: center top;
  background-repeat: no-repeat;
  background-size: cover;
  text-align: center;
  padding: 78px;
}
</style>