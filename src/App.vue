<template>
  <div id="app">
    <LoadApp />
    <HeaderApp />
    <HeroApp/>
  </div>
</template>

<script>
import LoadApp from "./components/LoadApp.vue";
import HeaderApp from "./components/HeaderApp.vue";
import HeroApp from "./components/HeroApp.vue";
export default {
  name: "App",
  components: {
    LoadApp,
    HeaderApp,
    HeroApp
}
};
</script>

<style lang="scss">
body {
  overflow: hidden;
}
</style>
