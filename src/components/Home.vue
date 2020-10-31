<template>
  <div>
    <h1 class="home">Class and style Binding</h1>
    <h1 v-bind:style="{color: 'blue'}">inline style</h1>
    <h1 v-bind:class="{display:show}">class Binding with Objects</h1>
    <h1 v-bind:class="[aclass]">Class binding with array</h1>
  </div>
</template>
<script>
export default {
  name: "Home",
  data() {
    return {
      show: true,
      aclass: "arrayClass"
    };
  }
};
</script>

<style scoped>
.home {
  color: orange;
}
.display {
  background-color: crimson;
}
.arrayClass {
  background-color: cyan;
}
</style>