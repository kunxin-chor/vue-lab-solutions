<template>
  <div id="app">
    <input type="text" v-model="msg"/>
    <span v-if="msg==''">Please type in something</span>
    <span v-if="msg && msg.length < 7">Too short</span>
    <span v-if="msg.length >= 7">OK</span>
  </div>
</template>

<script>

export default {
  name: 'App',
  data:function(){
    return {
      msg:""
    }
  },
  components: {
   
  }
}
</script>


