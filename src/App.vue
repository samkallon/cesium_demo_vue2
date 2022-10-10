<template>
  <div id="app">
    <left-menu class="left-menu"></left-menu>
    <CesiumViewer class="cesium-viewer"></CesiumViewer>
  </div>
</template>

<script>
import LeftMenu from "@/components/LeftMenu";
import CesiumViewer from "@/components/CesiumViewer";

export default {
  name: 'App',
  components: {
    CesiumViewer,
    LeftMenu
  }
}
</script>

<style lang="scss" scoped>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  width: 100%;
  height: 100%;
  display: flex;
  .left-menu{
    flex-grow: 1;
  }
  .cesium-viewer{
    flex-grow: 10;
  }
}
</style>
