<template>
  <div>
    <Nav />

    <main class="py-4">
      <router-view @loggedIn="change"></router-view>
    </main>

  </div>
</template>
<script>
import Nav from "./Nav";

export default {
  data() {
    return {
      name: null,
      user_type: 0,
      isLoggedIn: localStorage.getItem("jwt") != null,
    };
  },

  components: {
    Nav
  },
  mounted() {
    this.setDefaults();
  },
  methods: {
    setDefaults() {
      if (this.isLoggedIn) {
        let user = JSON.parse(localStorage.getItem("user"));
        this.name = user.name;
        this.user_type = user.is_admin;
      }
    },
    change() {
      this.isLoggedIn = localStorage.getItem("jwt") != null;
      this.setDefaults();
    },
    logout() {
      localStorage.removeItem("jwt");
      localStorage.removeItem("user");
      this.change();
      this.$router.push("/");
    },
  },
};
</script>