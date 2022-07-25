<template>
  <div id="app">
    <div v-bind:style="{backgroundColor: bgcolor, height: height + 'px', width: width + 'px'}"></div>
    <button v-on:click="increaseHeight">Increase Height</button>
    <button v-on:click="increaseWidth">Increase Width</button>
    <button v-on:click="switchRed">Red Background</button>
    <button v-on:click="switchBlue">Blue Background</button>
    <button v-on:click="reset">Reset</button>
  </div>
</template>

<script>
export default {
  name: "App",
  data: function () {
    return {
      bgcolor: "gray",
      width: 50,
      height: 50,
    };
  },
  methods:{
    increaseHeight:function(){
      this.height += 10;
    },
    increaseWidth:function(){
      this.width += 10;
    },
    switchRed:function(){
      this.bgcolor = 'red'
    },
    switchBlue:function(){
      this.bgcolor = 'blue'
    },
    reset:function(){
      this.bgcolor = 'gray';
      this.height = 50;
      this.width = 50;
    }
  },
  components: {},
};
</script>

<style scoped>

</style>
