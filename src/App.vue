<template>
  <div class="flex w-screen h-screen ">
    <Background />
    <Login />
  </div>
</template>

<script>
import Background from "./components/Background.vue";
import Login from "./components/Login.vue";

export default {
  name: "App",
  components: {
    Background,
    Login,
  },
};
</script>

<style scoped></style>
