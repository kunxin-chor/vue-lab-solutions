<template>
  <div id="app">
    <div id="lights" v-bind:style="{backgroundColor: lightColor}">
    </div>
    <input type="radio" value="red" v-model="lightColor"/><label>Red</label>
    <input type="radio" value="green" v-model="lightColor"/><label>Green</label>
    <input type="radio" value="yellow" v-model="lightColor"/><label>Yellow</label>
  </div>
</template>

<script>

export default {
  name: 'App',
  data:function() {
    return {
      "lightColor":"white"
    }
  },
  components: {
   
  }
}
</script>

<style scoped>
#lights {
  background-color: white;
  height: 50px;
  width: 50px;
  border: 1px solid black;
}
</style>


