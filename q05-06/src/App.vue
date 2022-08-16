<template>
  <div id="app">
    <input type="checkbox" value="a" v-model="selectedCheck" /><label>A</label>
    <input type="checkbox" value="b" v-model="selectedCheck" /><label>B</label>
    <input type="checkbox" value="c" v-model="selectedCheck" /><label>C</label>
    <input type="checkbox" value="d" v-model="selectedCheck" /><label>D</label>
    <input type="checkbox" value="e" v-model="selectedCheck" /><label>E</label>
    <input type="checkbox" value="f" v-model="selectedCheck" /><label>F</label>
    <div id="result">{{ selectedCheck.length }}</div>
  </div>
</template>

<script>
export default {
  name: "App",
  data: function () {
    return {
      selectedCheck: [],
    };
  },
  components: {},
};
</script>


