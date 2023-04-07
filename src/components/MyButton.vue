<template>
  <!-- there is no difference between v-on:click and @click -->
  <button @click="showAlertInfo()">Button1, click me</button>
  <!-- you can pass some data to button -->
  <!-- method param by calling method in component, it MUST BE IN SINGLE QUOTE, NOT DOUBLE QUOTE! -->
  <button v-on:click ="showAlertInfoWithParam('Hello from Button2')">Button2, click me</button>
  <!-- a button for double click -->
  <button v-on:dblclick="showAlertInfo()">Button3, double click me</button>
  <!-- a mousemove event -->
  <h1 v-on:mousemove="showLogInfo()">Move you mouse over here</h1>
  <!-- build a button4, and how many times it has been clicked show be shown below -->
  <button @click="increaseCount()">Button4</button>
  <h2>A counter, how many times i clicked Button4: {{count}}</h2>
</template>

<script>
export default {
  name: "MyButton",
  data () {
    return {
      count: 0
    }
  },
  methods: {
    showAlertInfo() {
      alert("some alert info");
    },
    showAlertInfoWithParam(greetingFromButton) {
      alert("some alert info: " + greetingFromButton);
    },
    showLogInfo() {
      console.log("some console log info");
    },
    increaseCount() {
      //this key word "this", you cann in methods property access the field in data!
      this.count++;
    }
  }
}
</script>