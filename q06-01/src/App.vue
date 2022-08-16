<template>
  <div id="app">
    <input type="text" v-model="num1"/>
    <input type="text" v-model="num2"/>
    <div id="results">{{sum}}</div>
  </div>
</template>

<script>

export default {
  name: 'App',
  data:function(){
    return {
      num1: 0,
      num2: 0
    }
  },
  components: { 

   
  },
  computed: {
    sum() {
      return parseInt(this.num1) + parseInt(this.num2);
    }
  }
}
</script>


