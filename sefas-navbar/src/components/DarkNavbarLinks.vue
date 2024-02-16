<template>
  <template v-for="link in links" :key="link.name">
    <div v-if="!link.menu" class="p-3 navdarklink">{{ link.name }}</div>
    <div v-else-if="link.menu" class="dropdown">
      <div class="p-3 navdarklink">{{ link.name }}</div>
      <div class="dropdown-menu">
        <div v-for="menu in link.menu" class="px-4 py-2">{{ menu }}</div>
      </div>
    </div>
  </template>
</template>

<script>
export default {
  name: "DarkNavbarLinks",
  data() {
    return {
      // links: [
      //   "Activities",
      //   "Relationships",
      //   "Transactions",
      //   "Inventory",
      //   "Settings",
      //   "Report",
      // ],
      links: [
        {
          name: "Activities",
        },
        {
          name: "Relationships",
        },
        {
          name: "Transactions",
        },
        {
          name: "Inventory",
        },
        {
          name: "Settings",
          menu: ["Users", "Roles", "Employee"],
        },
        {
          name: "Report",
        },
      ],
    };
  },
};
</script>
<style scoped>
.navdarklink:hover {
  background-color: #f36c21;
}

.dropdown {
  position: relative;
}

.dropdown-menu {
  display: none;
  position: absolute;
  top: 100%;
  left: 0;
  background-color: white;
  z-index: 1;
}

.dropdown:hover .dropdown-menu {
  display: block;
}
</style>