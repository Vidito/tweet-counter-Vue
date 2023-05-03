<template>
  <TheHome msg="Tweet Counter" />
  <TheForm />
</template>

<script>
import TheHome from "./components/TheHome.vue";
import TheForm from "./components/TheForm.vue";

export default {
  name: "App",
  components: {
    TheHome,
    TheForm,
  },
};
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin: 10rem auto;
  max-width: 25rem;
  background-color: #233067;
  padding: 4rem 1rem;
  border-radius: 10px;
}
</style>
