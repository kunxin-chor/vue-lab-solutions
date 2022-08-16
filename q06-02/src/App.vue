<template>
  <div id="app">
    <input type="text" v-model="message"/>
    <div id="count">{{count}}</div>
  </div>
</template>

<script>

export default {
  name: 'App',
  data:function(){
    return {
      message:""
    }
  },
  computed:{
    count() {
      return this.message.length;
    }
  },
  components: {
   
  }
}
</script>


