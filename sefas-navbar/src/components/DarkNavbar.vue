<template>
  <nav class="navbar bg-333333 text-white justify-content-start px-4 py-0">
    <div><i class="fa-solid fa-house-chimney px-2"></i></div>
    <DarkNavbarLinks></DarkNavbarLinks>
  </nav>
</template>

<script>
import DarkNavbarLinks from "./DarkNavbarLinks.vue";
export default {
  name: "DarkNavbar",
  components: {
    DarkNavbarLinks,
  },
};
</script>

<style>
</style>