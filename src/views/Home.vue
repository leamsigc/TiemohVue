<template>
  <div class="home">
    <Hero />
  </div>
</template>
<script lang="ts">
/**
 * HOME view and all related components
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
import Hero from "@/components/Hero.vue";
@Component({
  name: "Home",
  components: {
    Hero
  }
})
export default class Home extends Vue {
  /******Props *****/
  /******Vuex *****/
  /******localState *****/
  /*****  HelperFunction ******/
  /*****  Methods ******/
}
</script>
<style lang="scss" scoped></style>
