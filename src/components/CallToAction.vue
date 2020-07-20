<script lang="ts">
/**
 * Call to action for the users
 *
 * @author Reflect-Media <reflect.media GmbH>
 * @version 0.0.1
 *
 * @todo [ ] Test the component
 * @todo [ ] Integration test.
 * @todo [✔] Update the typescript.
 */

import { Vue, Component } from "vue-property-decorator";
// import { mapGetters, mapActions } from "vuex";

@Component({
  name: "CallToAction"
})
export default class CallToAction extends Vue {
  /******Props *****/
  /******Vuex *****/
  /******localState *****/
  /*****  HelperFunction ******/
  /*****  Methods ******/
}
</script>

<template>
  <div class="container">
    <div class="action">
      <h2 class="title-sub">Won't miss early-bird offers</h2>
      <form @submit.prevent class="form">
        <div class="input-container">
          <input class="form-input" type="text" placeholder="Full name" />
          <input
            class="form-input"
            type="email"
            placeholder="example@email.com"
          />
        </div>
        <div class="call-container">
          <button class="btn" type="submit">Claim my early access</button>
        </div>
      </form>
    </div>
    <small class="small text-muted">
      terms By clicking "Claim my early access", you agree to our statement and
      <span class="text-focus">privacy</span> .
    </small>
  </div>
</template>
<style lang="scss" scoped>
.container {
  width: 100%;
}
.action {
  margin-top: 4rem;
  .form {
    display: flex;
    justify-content: space-between;
    margin-top: 1rem;
    .input-container {
      flex: 1 0 0;
      display: flex;
      justify-content: start;
      align-items: center;
    }
    &-input {
      display: block;
      flex: 35% 0 1;
      background: var(--white-color);
      padding: 1.7rem 2rem;
      margin-right: 0.2rem;
      border: 0;
    }
    .btn {
      display: block;
      padding: 1.5rem 4rem;
      border: 1px solid transparent;
      border-radius: 5px;
      color: var(--white-color);
      background: var(--primary-color);
      font-size: 1rem;
      font-weight: 900;
    }
  }
}
.text-focus {
  font-weight: normal;
}
.title-sub {
  color: var(--text-color);
  font-weight: normal;
}
.small {
  display: block;
  margin-top: 0.5rem;
}
</style>
