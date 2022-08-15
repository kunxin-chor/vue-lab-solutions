<template>
  <div id="app">
    <traffic-light v-bind:signal='status'></traffic-light>
    <button v-on:click="go">Go</button>
    <button v-on:click="wait">Wait</button>
    <button v-on:click="stop">Stop</button>
  </div>
</template>

<script>
import TrafficLight from '@/TrafficLight.vue'

export default {
  name: 'App',
  data:function(){
    return {
      status:''
    }
  },
  methods:{
    go:function(){
      this.status = 'go'
    },
    wait:function(){
      this.status='wait'
    },
    stop:function(){
      this.status='stop'
    }
  },
  components: {
    TrafficLight
  }
}
</script>