<template>
  <div id="app">
    <router-view />
    <div class="navigation-footer">
      <Navbar />
    </div>
  </div>
</template>


<script>
import Navbar from "./components/Navbar.vue";
export default {
  name: "App",
  components: {
    Navbar
  }
};
</script>
<style>
@import "css/App.css";
</style>
