<template>
  <div id="app">
    <div class="box" v-bind:style="{backgroundColor:bgcolor}"></div>
    <button v-on:click="switchRed">Red</button>
    <button v-on:click="switchGreen">Green</button>
    <button v-on:click="switchBlue">Blue</button>
  </div>
</template>

<script>
export default {
  name: "App",
  data: function () {
    return { bgcolor: "" };
  },
  methods: {
    switchRed:function(){
      this.bgcolor = 'red'
    },
    switchBlue:function(){
      this.bgcolor = 'blue'
    },
    switchGreen:function(){
      this.bgcolor = 'green'
    }
  },
  components: {},
};
</script>

<style scoped>
.box {
  width: 50px;
  height: 50px;
  border: 1px solid black;
}
</style>

