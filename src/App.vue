<template>
  <div id="app">
    <LoadApp />
    <HeaderApp />
    <HeroApp/>
    <SellApp/>
    <ActionsApp/>
    <FeatureApp/>
    <HotApp/>
    <CreateApp/>
    <FooterApp/>
  </div>
</template>

<script>
import LoadApp from "./components/LoadApp.vue";
import HeaderApp from "./components/HeaderApp.vue";
import HeroApp from "./components/HeroApp.vue";
import SellApp from "./components/SellApp.vue";
import ActionsApp from "./components/ActionsApp.vue";
import FeatureApp from "./components/FeatureApp.vue";
import HotApp from "./components/HotApp.vue";
import CreateApp from "./components/CreateApp.vue";
import FooterApp from "./components/FooterApp.vue";

export default {
  name: "App",
  components: {
    LoadApp,
    HeaderApp,
    HeroApp,
    SellApp,
    ActionsApp,
    FeatureApp,
    HotApp,
    CreateApp,
    FooterApp
}
};
</script>

<style lang="scss">
  @import url('../WEB/css/chillax.css');
body {
  overflow: hidden;
}
</style>
