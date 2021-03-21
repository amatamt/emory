<template>
  <div class="container">
    <div>
      <h1 class="title">
        <b>emory</b>
      </h1>
      <b-form>
        <b-form-group
          id="input-group-1"
          label="Sign in with your emory ID"
          label-for="input-1"
        >
          <b-form-input
            id="input-1"
            placeholder="emory ID"
          ></b-form-input>
        </b-form-group>

        <b-form-group id="input-group-2" label-for="input-2">
          <b-form-input
            id="input-2"
            type="password"
            placeholder="password"
          ></b-form-input>
        </b-form-group>

        <b-button @click="login" variant="success">Sign In</b-button>
      </b-form>
    </div>
  </div>
</template>

<script lang="ts">
import Vue from 'vue'

export default Vue.extend({
  methods: {
    login() {
      console.log("login")
      this.$router.push('/home')
    }
  }
})
</script>

<style>
.container {
  margin: 0 auto;
  min-height: 100vh;
  display: flex;
  justify-content: center;
  align-items: center;
  text-align: center;
}

.title {
  font-family:
    'Quicksand',
    'Source Sans Pro',
    -apple-system,
    BlinkMacSystemFont,
    'Segoe UI',
    Roboto,
    'Helvetica Neue',
    Arial,
    sans-serif;
  display: block;
  font-weight: 300;
  font-size: 100px;
  color: #35495e;
  letter-spacing: 1px;
}

.subtitle {
  font-weight: 300;
  font-size: 42px;
  color: #526488;
  word-spacing: 5px;
  padding-bottom: 15px;
}

.links {
  padding-top: 15px;
}
</style>
