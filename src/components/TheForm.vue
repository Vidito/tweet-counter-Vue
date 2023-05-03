<script>
export default {
  name: "TheForm",
  data() {
    return {
      tweet: "",
    };
  },
};
</script>

<template>
  <div class="form">
    <textarea
      v-model="tweet"
      name="tweet"
      type="text"
      placeholder="Tweet here"
    />
    <p v-if="tweet.length < 281" class="green">
      👍 {{ tweet.length }} characters
    </p>
    <p v-else class="red">👎 {{ tweet.length }} characters</p>
    <h3>It will appear as:</h3>
    <textarea disabled> {{ tweet.slice(0, 280) }} </textarea>
  </div>
</template>

<style scoped>
textarea {
  width: 100%;
  height: 150px;
  padding: 12px 20px;
  box-sizing: border-box;
  border: 2px solid #ccc;
  border-radius: 4px;
  background-color: #f8f8f8;
  font-size: 16px;
  resize: none;
}
textarea:focus {
  outline: none;
}
p,
h3 {
  color: white;
}
.green {
  color: green;
}
.red {
  color: red;
}
</style>