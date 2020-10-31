<template>
  <div>
    <h1>Child componet</h1>
    <h3 v-for="user in users" :key="user.name">{{user.name}}</h3>
  </div>
</template>

<script>
export default {
  name: "Child",
  props: ["users"]
};
</script>