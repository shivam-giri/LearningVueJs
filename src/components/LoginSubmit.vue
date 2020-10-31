<template>
  <div>
      <p v-if="error.length">
          <b>Please correct the following error</b>
          <ul>
              <li v-for=" e in error" v-bind:key="e.id" >
                  {{e}}
              </li>
          </ul>
      </p>
    <form @submit="login">
      <input type="text" placeholder="user name" v-model="name" />
      <br />
      <br />
      <input type="password" placeholder="password here" v-model="password" />
      <br />
      <br />
      <button type="submit">Login Here</button>
    </form>
  </div>
</template>

<script>
export default {
  name: "Login",
  data() {
    return {
      error: [],
      name: null,
      password: null
    };
  },
  methods: {
    login(e) {
      if (this.name && this.password) {
        console.warn("no error");
        return true;
      }
      if (!this.name) {
        this.error.push("User name is required");
      }

      if (!this.password) {
        this.error.push("password is required");
      }
      console.warn("hello", this.error);
      e.preventDefault();
    }
  }
};
</script>