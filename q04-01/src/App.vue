<template>
  <div id="app">
    <message-box msg="Mary has a little lamb"/>
  </div>
</template>

<script>
import MessageBox from '@/components/MessageBox.vue'
export default {
  name: 'App',
  components: {    
    MessageBox
  }
}
</script>


