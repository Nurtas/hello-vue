<template>
<div>{{ greet }} {{ name }}</div>
<div v-text="channel"></div>
<div v-html="bold_text"></div>
<div v-html="hack"></div>
<h2 v-bind:id="headingId">Heading</h2>
<button v-bind:disabled="isDisabled">Button</button>
</template>

<script>
export default {
  name: 'App',
  data() {
    return {
      greet: "Hello",
      name: "Nurtas",
      channel: "Code Snippet",
      bold_text: "<b>bold</b>",
      hack: `<a href="#" onClick="alert('You have been hacked!')">Win a prize!</a>`,
      headingId: 'heading',
      isDisabled: false,
    }
  }
}
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
