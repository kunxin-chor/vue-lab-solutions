<template>
  <div id="app">
    <span v-bind:style="{fontSize: textSize + 'px'}">Hello World</span>
    <button v-on:click="increase">Increase</button>
    <button v-on:click="decrease">Decrease</button>
  </div>
</template>

<script>

export default {
  name: 'App',
  data:function(){
    return {
      'textSize':12
    }
  },
  methods:{
    'increase':function(){
      this.textSize += 5
    },
    'decrease':function(){
      this.textSize -= 5;
    }
  },
  components: {
   
  }
}
</script>


