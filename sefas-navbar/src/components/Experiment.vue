<template>
  <ul class="navbar">
    <li><a href="#">Home</a></li>
    <li class="dropdown">
      <a href="#">Products</a>
      <ul class="dropdown-menu">
        <li><a href="#">Product 1</a></li>
        <li><a href="#">Product 2</a></li>
      </ul>
    </li>
    <li><a href="#">Contact</a></li>
  </ul>
</template>

<script>
export default {
  name: "Experiment",
};
</script>

<style>
.navbar {
  list-style: none;
  margin: 0;
  padding: 0;
}

.navbar li {
  display: inline-block;
  margin-right: 10px;
}

.navbar li a {
  display: block;
  padding: 10px;
  text-decoration: none;
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