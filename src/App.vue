<template>
  <div id="app">
    <Header></Header>
    <add-countdown-btn></add-countdown-btn>
    <counter-card  v-for="(cnt, index) in cnts" :key="index"></counter-card>
    
  </div>
</template>

<script>
import Header from "./components/Header.vue";
import CounterCard from "./components/CounterCard.vue";
import AddCountdownBtn from "./components/AddCountdownBtn"
export default {
  name: "App",
  components: {
    Header,
    CounterCard,
    AddCountdownBtn
  },
  data() {
    return{
      cnts: [{
        index: '1'
      }, {
        index: '2'
      }]
    }
  }
};
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: left;
  color: #2c3e50;
}
</style>
