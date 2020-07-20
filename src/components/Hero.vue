<template>
  <div class="hero">
    <div class="hero-text">
      <div class="container">
        <h1 class="title-main">
          <span class="text-focus">Missing</span>
          your lovely
          <br />
          <span class="text-focus">home</span>country
          <br />
          <span class="text-focus">food ?</span>
        </h1>
        <p class="text-info">
          Well say no more, we at
          <span class="text-focus">TIEMOH</span> help to connect you to the
          people from your home country that are traveling and are open to bring
          your home country ingredients and spices to you.
        </p>
        <p class="text-info">
          When the food test like home everything is better.
        </p>
      </div>
      <CallToAction />
    </div>
  </div>
</template>

<script lang="ts">
import { Component, Prop, Vue } from "vue-property-decorator";
import CallToAction from "@/components/CallToAction.vue";
@Component({
  name: "Hero",
  components: {
    CallToAction
  }
})
export default class Hero extends Vue {
  @Prop() private msg!: string;
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
.hero {
  display: grid;
  grid-template-areas: "information information";
  position: relative;

  background: url("/img/hero/hero-bg-woman.png");
  background-repeat: no-repeat;
  background-position: left bottom;

  &-text {
    min-height: 100vh;
    grid-area: information;
    display: flex;
    justify-content: center;
    align-items: center;
    flex-direction: column;

    background: url("/img/hero/heroBg.png");
    background-repeat: no-repeat;
    background-position: 100%;
    background-size: 55%;
    color: var(--dark-color);
    .conatiner {
      display: flex;
      justify-content: center;
      flex-direction: column;
      align-items: baseline;
    }
    .title-main {
      font-size: 48px;
      font-weight: 500;
      text-align: center;
      max-width: 40%;
    }
    .text-info {
      margin-top: 2rem;
      max-width: 45%;
      text-align: center;
      line-height: 150%;
    }
  }
}
</style>
