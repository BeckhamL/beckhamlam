<template>
  <div>
    <b-navbar toggleable="sm" type="light" variant="light">
      <div class="container">
        <b-navbar-toggle target="nav-text-collapse"></b-navbar-toggle>

        <b-navbar-brand>BootstrapVue</b-navbar-brand>

        <b-collapse id="nav-text-collapse" is-nav>
          <b-navbar-nav>
            <b-nav-text>Navbar text</b-nav-text>
          </b-navbar-nav>
        </b-collapse>
      </div>
    </b-navbar>
  </div>
</template>

<script setup></script>

<style lang="scss" scoped></style>
