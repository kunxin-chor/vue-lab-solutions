<template>
  <div id="app">
    <div id="result">{{(parseInt(width)+parseInt(height))*2}}</div>
    <input type="text" v-model='width'/>
    <input type="text" v-model='height'/>
  </div>
</template>

<script>

export default {
  name: 'App',
  data:function(){
    return {
      'width': 0,
      'height': 0
    }
  },
  components: {
   
  }
}
</script>


