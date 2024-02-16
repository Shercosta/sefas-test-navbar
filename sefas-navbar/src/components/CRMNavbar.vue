<template>
  <nav class="navbar jc-sb px-4">
    <div><strong>CRM</strong></div>
    <div class="d-flex form-input">
      <div class="form-control">
        <input type="text" placeholder="Search..." class="border border-0" />
        <i class="fa-solid fa-magnifying-glass color-tertiary"></i>
      </div>
    </div>
    <div class="d-inline-flex color-tertiary">
      <div class="dropdown px-2">
        <a
          class="nav-link dropdown-toggle"
          href="#"
          role="button"
          data-bs-toggle="dropdown"
          aria-expanded="false"
        >
          <i class="fa-regular fa-file-lines"></i>
        </a>
      </div>
      <div class="dropdown px-2">
        <a
          class="nav-link dropdown-toggle"
          href="#"
          role="button"
          data-bs-toggle="dropdown"
          aria-expanded="false"
        >
          <i class="fa-solid fa-grip"></i>
        </a>
      </div>
      <div class="dropdown px-2">
        <a
          class="nav-link dropdown-toggle"
          href="#"
          role="button"
          data-bs-toggle="dropdown"
          aria-expanded="false"
        >
          <i class="fa-solid fa-user"></i>
        </a>
      </div>
    </div>
  </nav>
</template>

<script>
export default {
  name: "CRMNavbar",
};
</script>

<style>
</style>