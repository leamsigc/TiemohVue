<script lang="ts">
/**
 * All the nav bar information is handle in this component
 *
 * @author  ismael garcia  <reflect.media GmbH>
 * @version 0.0.1
 *
 * @todo [ ] Test the component
 * @todo [ ] Integration test.
 * @todo [✔] Update the typescript.
 */
import { Vue, Component } from "vue-property-decorator";
// import { mapGetters, mapActions } from "vuex";

@Component({
  name: "NavBar"
})
export default class NavBar extends Vue {
  /******Props *****/
  /******Vuex *****/
  /******localState *****/
  /*****  HelperFunction ******/
  /*****  Methods ******/
}
</script>

<template>
  <div id="nav" class="flex-container nav-bar">
    <div class="logo-container">
      <span class="logo">TIEMOH</span>
    </div>
    <div class="navigation-container">
      <router-link class="nav-link" to="/">Home</router-link>
      <router-link class="nav-link" to="/about">Services</router-link>
      <router-link class="nav-link" to="/about">Partners</router-link>
      <router-link class="nav-link" to="/about">Contact US</router-link>
    </div>
  </div>
</template>
<style scoped lang="scss">
.flex-container {
  display: flex;
  justify-content: space-between;
  padding-top: 2rem;
  max-width: 1200px;
  margin: 0 auto;
}
.nav-bar {
  position: absolute;
  top: 0;
  right: 0;
  left: 0;
  z-index: 200;
}
.logo-container {
  flex: 1 0 1;
}
.navigation-container {
  display: flex;
  justify-content: space-around;
  align-items: center;
  min-width: 50%;
}
.logo {
  font-size: 48px;
  font-weight: bold;
  color: var(--primary-color);
}
.nav-link {
  padding: 0.5rem 1rem;
  text-decoration: none;
  color: var(--text-color);
  font-weight: 600;
  transition: all 0.3s ease-in-out;
}
.nav-link:hover {
  color: var(--white-color);
  font-weight: bold;
  box-shadow: inset 0 -2.5rem 0 var(--text-color);
}
</style>
