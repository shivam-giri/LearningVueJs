<template>
  <div>
    <input type="text" v-model="loginForm.username" name="username" placeholder="name here" />
    <br />
    <br />
    <input type="password" v-model="loginForm.password" name="password" placeholder="password" />
    <br />
    <br />
    <button v-on:click="loginData">Login</button>
  </div>
</template>

<script>
export default {
  name: "Login",
  methods: {
    loginData() {
      console.log(
        "loginData",
        this.loginForm.username,
        this.loginForm.password
      );
    }
  },
  data() {
    return {
      loginForm: {
        username: null,
        password: null
      }
    };
  }
};
</script>