<template>
  <div id="app">
    <!-- <img alt="Vue logo" src="./assets/logo.png"> -->
    <HelloWorld msg="Welcome to Your Vue.js App"/>
  </div>
</template>

<script>
import HelloWorld from './components/HelloWorld.vue'

export default {
  name: 'app',
  components: {
    HelloWorld
  }
}
</script>

<style lang="scss">
    // 1. Your custom variables and variable overwrites.
    $global-link-color: #DA7D02;
    // 2. Import default variables and available mixins.
    @import "~uikit/src/scss/variables-theme.scss";
    @import "~uikit/src/scss/mixins-theme.scss";
    // 3. Your custom mixin overwrites.
    @mixin hook-card() {
        color: #000;
    }
    // 4. Import UIkit.
    @import "~uikit/src/scss/uikit-theme.scss";
    // Some font smoothing
    html {
        -webkit-font-smoothing: antialiased;
        -moz-osx-font-smoothing: grayscale;
        text-rendering: optimizeLegibility;
    }
</style>
