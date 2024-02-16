<template>
  <template v-for="link in links" :key="link">
    <div class="p-3 navdarklink">{{ link }}</div>
  </template>
</template>

<script>
export default {
  name: "DarkNavbarLinks",
  data() {
    return {
      links: [
        "Activities",
        "Relationships",
        "Transactions",
        "Inventory",
        "Settings",
        "Report",
      ],
    };
  },
};
</script>
<style scoped>
.navdarklink:hover {
  background-color: #f36c21;
}
</style>