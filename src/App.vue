<template>
  <div id="app">
    <PfGlobalNavi />
    <router-view />
    <PfGlobalFooter />
  </div>
</template>

<script>
import PfGlobalNavi from "@/components/Molecules/PfGlobalNavi.vue";
import PfGlobalFooter from "@/components/Molecules/PfGlobalFooter.vue";
export default {
  components: {
    PfGlobalNavi,
    PfGlobalFooter
  }
};
</script>

<style>
body {
  max-width: 1920px;
  margin: auto;
}
#app {
  width: 100%;
  margin: auto;
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
}
</style>
