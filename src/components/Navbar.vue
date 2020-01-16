<template>
  <div class="nav">
    <div class="line"></div>
    <router-link
      v-for="(nav, key) in nav_list"
      v-bind:key="key"
      v-bind:to="{path: nav.route}"
    >{{nav.title}}</router-link>
  </div>
</template>

<script>
// @ is an alias to /src

export default {
  name: "Navbar",
  components: {},
  data() {
    return {
      nav_list: [
        { title: "Home", route: "/home" },
        { title: "My Work", route: "/work" },
        { title: "About", route: "/about" },
        { title: "Contact", route: "/contact" }
      ]
    };
  }
};
</script>

<style scoped>
@import "../css/Navbar.css";
</style>