<template>
  <div id="app">
    <!-- <SignUp /> -->
    <!-- <Login /> -->
    <!-- <LoginSubmit />  -->
    <EmployeeList />
  </div>
</template>

<script>
import EmployeeList from "./components/EmployeeList";
// import LoginSubmit from "./components/LoginSubmit";
// import Login from "./components/Login";
// import SignUp from "./components/SignUp";
export default {
  name: "App",
  components: {
    // SignUp
    // Login
    // LoginSubmit
    EmployeeList
  }
};
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
