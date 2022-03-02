<template>
  <div class="nov-row col-lg-12 col-xs-12">
    <div class="nov-row-wrap row">
      <Products/>
      <HotDeals/>
    </div>
  </div>
</template>
<script>
  import Products from "./Products";
  import HotDeals from "./HotDeals";
export default {

  data() {
    return {
      className: "owl-item active firstActiveItem",
    };
  },
    components: {
    Products,
    HotDeals,
  }
 
};
</script>