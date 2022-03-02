<template>
  <div>
    <aside id="notifications">
      <div class="container"></div>
    </aside>
    <HeroCard />
    <div class="container">
      <div class="row">
        <Ads />
        <ListProducts />
        <Brands />
        <Ads2 />
       
      </div>
    </div>

    <Footer />
  </div>
</template>
<script>
import Nav from "./Nav";
import HeroCard from "./HeroCard";
import Ads from "./Ads";
import Ads2 from "./Ads2";
import ListProducts from "./ListPorducts";
import Footer from "./Footer";
import Brands from "./Brands";
import HotTreding from "./HotTreding";

export default {
  data() {
    return {
      name: null,
      user_type: 0,
      isLoggedIn: localStorage.getItem("jwt") != null,
    };
  },

  components: {
    Nav,
    HeroCard,
    Ads,
    Ads2,
    ListProducts,
    Footer,
    Brands,
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