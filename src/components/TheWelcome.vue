<template>
  <div>
    <div>
      <label for="inputText">Input Text:</label>
      <input type="text" id="inputText" v-model="inputText" @input="updateText">
    </div>
    <div :style="{ marginTop: '20px', fontSize: '18px' }">
      <p v-text="displayText"></p>
    </div>
  </div>
</template>

<script>
export default {
  data() {
    return {
      inputText: '',
      displayText: ''
    };
  },
  methods: {
    updateText() {
      this.displayText = this.inputText;
    }
  }
};
</script>

<style scoped>
/* Add your styles here */
</style>
