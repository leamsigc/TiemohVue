<script lang="ts">
/**
 * This is the amin entry for the aplication
 *
 * @author  ismael garcia  <reflect.media GmbH>
 * @version 0.0.1
 *
 * @todo [ ] Test the component
 * @todo [ ] Integration test.
 * @todo [✔] Update the typescript.
 */
import { Vue, Component } from "vue-property-decorator";
import NavBar from "@/components/NavBar.vue";
// import { mapGetters, mapActions } from "vuex";

@Component({
  name: "App",
  components: {
    NavBar
  }
})
export default class App extends Vue {
  /******Props *****/
  /******Vuex *****/
  /******localState *****/
  /*****  HelperFunction ******/
  /*****  Methods ******/
}
</script>
<template>
  <div id="app">
    <NavBar />
    <router-view />
  </div>
</template>

<style lang="scss">
:root {
  --primary-color: #49059f;
  --main-white-bg: #fff;
  --white-color: #e5e5e5;
  --muted-text: #b8b8b8;
  --dark-color: #140b1f;
  --text-color: #3d3d3d;

  // main font
  --main-font: "Montserrat", sans-serif;
}
* {
  display: 0;
  margin: 0;
  box-sizing: border-box;
}
html,
body {
  font-family: var(--main-font);
  background: var(--main-white-bg);
}
#app {
  position: relative;
}
.container {
  max-width: 1200px;
  margin: 0 auto;
}
.text-muted {
  color: var(--muted-text);
}
.text-focus {
  color: var(--primary-color);
  font-weight: 900;
}
</style>
