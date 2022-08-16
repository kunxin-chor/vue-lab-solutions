<template>
  <div id="app">
    <div id="lights" v-bind:style="{backgroundColor:lightColor}">
    </div>
    <select v-model="lightColor">
      <option value="red">Red</option>
      <option value="green">Green</option>
      <option value="yellow">Yellow</option>
    </select>
  </div>
</template>

<script>

export default {
  name: 'App',
  data: function() {
    return {
      'lightColor': 'white'
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


