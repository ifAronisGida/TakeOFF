<template>
  <div>
    <b-navbar fixed="top" toggleable="lg" type="light" variant="light" >
      <b-navbar-brand :to="{ name: 'Home' }">TakeOff</b-navbar-brand>
      <b-navbar-toggle target="nav-collapse"></b-navbar-toggle>
      <b-collapse id="nav-collapse" is-nav>
        <b-navbar-nav>
          <b-nav-item href="#">Retro</b-nav-item>
          <b-nav-item href="#">Tegnap</b-nav-item>
        </b-navbar-nav>

        <!-- Right aligned nav items -->
        <b-navbar-nav class="ml-auto">

          <b-nav-item-dropdown right>
            <!-- Using 'button-content' slot -->
            <template slot="button-content"><em>User</em></template>
            <b-dropdown-item href="#">Profile</b-dropdown-item>
            <b-dropdown-item href="#">Sign Out</b-dropdown-item>
          </b-nav-item-dropdown>
        </b-navbar-nav>
      </b-collapse>
    </b-navbar>
  </div>
</template>
<script>
import Datepicker from 'vuejs-datepicker';
import PostService from '@/api-services/post.service';

export default {
  name: 'Navbar',
  components: { Datepicker },
  data() {
    return {
      date: new Date(Date.now()),
    };
  },
  methods: {
    onClick() {
      PostService.create({ Id: 1, Description: 'this is a journal' });
    },
  },

};
</script>

<style scoped>

</style>
