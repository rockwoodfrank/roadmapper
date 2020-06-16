<template>
  <div id="app">
    <Header />
    <router-view />
  </div>
</template>

<script>
import Header from "@/components/Header";

import "@/assets/frameworks.css";

export default {
  name: "App",
  components: {
    Header
  }
};
</script>

<style lang="scss">
* {
  margin: 0;
  padding: 0;
}
body {
  font-family: "Rubik", sans-serif;
}
</style>
