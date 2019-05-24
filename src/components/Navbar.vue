<template>
  <b-navbar
    toggleable="md"
    type="dark"
    variant="info">
    <b-navbar-brand :to="{ name: 'Home' }">TakeOff Home</b-navbar-brand>
    <b-navbar-nav>
      <b-nav-item href="#">navitem1</b-nav-item>
      <b-nav-item href="#">navitem2</b-nav-item>
      <b-nav-item href="#">navitem3</b-nav-item>
    </b-navbar-nav>
  </b-navbar>
</template>
<script>
export default {
  name: 'Navbar',
};
</script>

<style scoped>

</style>
