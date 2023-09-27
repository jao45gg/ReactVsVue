<template>
  <div id="app">
    <p id="p1">You clicked {{ numOfClicks }} times.</p>
    <button id="btn1" @click="clickCount()">Add +1</button>
    <button id="btn2" @click="clearAll">Reset</button>
  </div>
</template>

<script>
console.log("Options API RENDER");
export default {
  name: "App",
  data() {
    return { numOfClicks: 0 };
  },
  created() {},
  methods: {
    clickCount: function () {
      this.numOfClicks++;
    },
    clearAll: function () {
      this.numOfClicks = 0;
    },
  },
};
</script>

<style>
@import "./style.css";
</style>
