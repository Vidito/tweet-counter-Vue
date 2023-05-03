<template>
  <h1>{{ msg }}</h1>
  <p>Enter Your Tweet For The Counter</p>
  <TheForm />
</template>

<script>
export default {
  name: "TheHome",
  props: {
    msg: {
      type: String,
      required: true,
    },
  },
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
h1 {
  color: #ef2e2f;
}
p {
  color: #fefefe;
}
</style>
