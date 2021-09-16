<template>
  <div>
    <b-navbar toggleable="lg" type="dark" variant="info">
      <nuxt-link class="navbar-brand" to="/">NavBar</nuxt-link>

      <b-navbar-toggle target="nav-collapse"></b-navbar-toggle>

      <b-collapse id="nav-collapse" is-nav>
        <b-navbar-nav class="ml-auto">
          <nuxt-link class="nav-link" active-class="active" to="/products"
            >Products</nuxt-link
          >
          <nuxt-link class="nav-link" active-class="active" to="/my-items"
            >My Item</nuxt-link
          >
        </b-navbar-nav>
      </b-collapse>
    </b-navbar>
  </div>
</template>

<script>
export default {};
</script>

<style>
</style>