<template>
  <div>
    <input type="text" placeholder="enter your name" v-model="signup.username" />
    <br />
    <input type="password" placeholder="password" v-model="signup.password" />
    <br />
    <p>Choose game</p>
    <input type="checkbox" name="cricket" id="cricket" value="cricket" v-model="signup.hobbies" />
    <label for="cricket">Cricket</label>
    <br />
    <input type="checkbox" id="football" value="football" v-model="signup.hobbies" />
    <label for="footbal">Football</label>

    <br />

    <p>choose gender</p>
    <input type="radio" name="male" id="male" value="male" v-model="signup.gender" />
    <label for="male">male</label>
    <br />
    <input type="radio" id="female" value="female" v-model="signup.gender" />
    <label for="female">Female</label>
    <br />
    <button v-on:click="signup">SignUpUser</button>
  </div>
</template>

<script>
export default {
  name: "SignUp",
  data() {
    return {
      signup: {
        username: null,
        password: null,
        hobbies: [],
        gender: null
      }
    };
  },
  methods: {
    SignUpUser() {
      console.warn(this.signup);
    }
  }
};
</script>
