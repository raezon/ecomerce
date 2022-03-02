<template>
  <div class="col-xl-9 col-lg-9 col-md-9 col-xs-12 col-md-12">
    <div class="block block-producttab" id="producttab1963514388">
      <div
        class="
          block-tab-title
          d-flex
          align-items-center
          justify-content-between
        "
      >
        <ul class="nav nav-tabs justify-content-center" role="tablist">
          <li class="nav-item">
            <a
              href="#producttab1963514388newproducts"
              class="nav-link active"
              role="tab"
              data-toggle="tab"
              aria-expanded="true"
              >New Arrivals</a
            >
          </li>
          <li class="nav-item">
            <a
              href="#producttab1963514388bestseller"
              class="nav-link"
              role="tab"
              data-toggle="tab"
              aria-expanded="false"
              >Best Seller</a
            >
          </li>
          <li class="nav-item">
            <a
              href="#producttab1963514388featured"
              class="nav-link"
              role="tab"
              data-toggle="tab"
              aria-expanded="false"
              >Featured</a
            >
          </li>
        </ul>
      </div>
      <div class="block_content">
        <div class="product_tab_content tab-content">
          <div
            class="tab-pane fade active in"
            id="producttab1963514388newproducts"
            aria-expanded="true"
          >
            <div
              id="producttab1963514388-newproducts"
              class="
                product_list
                grid
                owl-carousel owl-theme owl-loaded owl-drag
              "
              data-autoplay="false"
              data-autoplaytimeout="6000"
              data-loop="true"
              data-margin="0"
              data-dots="false"
              data-nav="true"
              data-items="3"
              data-items_large="3"
              data-items_tablet="2"
              data-items_mobile="2"
            >
              <div class="col-md-12">
                <div class="row">
                  <div
                    class="col-md-4 product-box"
                    v-for="(product, index) in products"
                    v-bind:key="index"
                  >
                    <div class="item text-center">
                      <!--Debut-->

                      <div
                        class="
                          product-miniature
                          js-product-miniature
                          item-one
                          first_item
                        "
                        data-id-product="16"
                        data-id-product-attribute="323"
                        itemtype="http://schema.org/Product"
                      >
                        <div class="thumbnail-container">
                          <a
                            href="http://demo.bestprestashoptheme.com/savemart/en/home-appliance/16-323-cras-consequat-quis-dolor-eunde.html#/1-size-s/11-color-black"
                            class="thumbnail product-thumbnail two-image"
                          >
                            <img
                              class="img-fluid image-cover"
                              :src="product.image"
                              :alt="product.name"
                              alt=""
                              data-full-size-image-url="http://demo.bestprestashoptheme.com/savemart/99-large_default/cras-consequat-quis-dolor-eunde.jpg"
                              width="600"
                              height="600"
                            />
                            <img
                              class="img-fluid image-secondary"
                              :src="product.image"
                              :alt="product.name"
                              alt=""
                              data-full-size-image-url="http://demo.bestprestashoptheme.com/savemart/100-large_default/cras-consequat-quis-dolor-eunde.jpg"
                              width="600"
                              height="600"
                            />
                          </a>

                          <div class="product-flags discount">Sale</div>
                        </div>

                        <div class="product-description">
                          <div class="product-groups">
                            <div class="category-title">
                              <a
                                href="http://demo.bestprestashoptheme.com/savemart/en/home-appliance/16-cras-consequat-quis-dolor-eunde.html"
                                >Home Appliance</a
                              >
                            </div>

                            <div class="product-comments">
                              <div class="star_content">
                                <div class="star"></div>
                                <div class="star"></div>
                                <div class="star"></div>
                                <div class="star"></div>
                                <div class="star"></div>
                              </div>
                              <span>0 review</span>
                            </div>
                            <p class="seller_name">
                              <a
                                title="View seller profile"
                                href="http://demo.bestprestashoptheme.com/savemart/en/jmarketplace/3_harry-makle/"
                              >
                                <i class="fa fa-user"></i>
                                {{ product.name }}
                              </a>
                            </p>

                            <div class="product-title" itemprop="name">
                              <a
                                href="http://demo.bestprestashoptheme.com/savemart/en/home-appliance/16-323-cras-consequat-quis-dolor-eunde.html#/1-size-s/11-color-black"
                              >
                                {{ product.name }}
                              </a>
                            </div>

                            <div class="product-group-price">
                              <div class="product-price-and-shipping">
                                <span itemprop="price" class="price">{{
                                  product.price
                                }}</span>

                                <span class="regular-price">{{
                                  product.price
                                }}</span>
                              </div>
                            </div>
                          </div>
                          <div
                            class="
                              product-buttons
                              d-flex
                              justify-content-center
                            "
                            itemprop="offers"
                            itemtype="http://schema.org/Offer"
                          >
                            <form
                              action="http://demo.bestprestashoptheme.com/savemart/en/cart"
                              method="post"
                              class="formAddToCart"
                            >
                              <input
                                type="hidden"
                                name="token"
                                value="28add935523ef131c8432825597b9928"
                              />
                              <input
                                type="hidden"
                                name="id_product"
                                value="16"
                              />
                              <a
                                class="add-to-cart"
                                href="#"
                                data-button-action="add-to-cart"
                                ><i class="novicon-cart"></i
                                ><span>Add to cart</span></a
                              >
                            </form>

                            <a
                              class="addToWishlist wishlistProd_16"
                              href="#"
                              data-rel="16"
                            >
                              <i class="fa fa-heart"></i>
                              <span>Add to Wishlist</span>
                            </a>
                            <a
                              href="#"
                              class="quick-view hidden-sm-down"
                              data-link-action="quickview"
                            >
                              <i class="fa fa-search"></i
                              ><span> Quick view</span>
                            </a>
                          </div>
                        </div>
                      </div>
                      <!-- Fin Produit-->
                    </div>
                  </div>
                </div>
              </div>
            </div>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>
<script>
  import Products from "./Products";
  import HotDeals from "./HotDeals";
export default {

  data() {
    return {
      products: [],
      className: "owl-item active firstActiveItem",
    };
  },
  mounted() {
    axios
      .get("api/products/")
      .then((response) => {
        this.products = response.data;
      })
      .catch((error) => {
        console.error(error);
      });
  },
};
</script>