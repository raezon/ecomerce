<template>
  <div>
    <header id="header" class="header-1 sticky-menu">
      <div class="header-mobile hidden-md-up">
        <div
          class="
            hidden-md-up
            text-xs-center
            mobile
            d-flex
            align-items-center
            justify-content-end
          "
        >
          <div id="_mobile_mainmenu" class="item-mobile-top">
            <i class="material-icons d-inline">menu</i>
          </div>
          <div class="mobile_logo ml-auto mr-auto">
            <a href="http://demo.bestprestashoptheme.com/savemart/">
              <img
                class="logo-mobile img-fluid"
                src="http://demo.bestprestashoptheme.com/savemart/modules/novthemeconfig/images/logo-mobile.png"
                alt="Prestashop_Savemart"
              />
            </a>
          </div>
          <div
            id="_mobile_menutop"
            class="
              item-mobile-top
              nov-toggle-page
              d-flex
              align-items-center
              justify-content-center
            "
            data-target="#mobile-pagemenu"
          >
            <i class="material-icons">more_horiz</i>
          </div>
        </div>

        <div id="_mobile_search"></div>
      </div>

      <div class="header-top hidden-sm-down">
        <div class="container">
          <div class="content">
            <div class="row">
              <div
                class="
                  header-top-left
                  col-lg-6 col-md-6
                  d-flex
                  justify-content-start
                  align-items-center
                "
              >
                <div
                  class="
                    detail-email
                    d-flex
                    align-items-center
                    justify-content-center
                  "
                >
                  <i class="icon-email"></i>
                  <p>Email :</p>
                  <span> support@gmail.com </span>
                </div>
                <div
                  class="
                    detail-call
                    d-flex
                    align-items-center
                    justify-content-center
                  "
                >
                  <i class="icon-deal"></i>
                  <p>Today Deals</p>
                </div>
              </div>
              <div
                class="
                  col-lg-6 col-md-6
                  d-flex
                  justify-content-end
                  align-items-center
                  header-top-right
                "
              >
                <ul class="register-out ml-auto">
                  <i class="zmdi zmdi-account"></i>
                  <li>
                    <router-link
                      :to="{ name: 'login' }"
                      class="login"
                      v-if="!isLoggedIn"
                      >Login</router-link
                    >
                  </li>
                  <span class="or-text">or</span>
                  <li>
                    <router-link
                      :to="{ name: 'register' }"
                      class="register"
                      v-if="!isLoggedIn"
                      >Register</router-link
                    >
                  </li>
                </ul>
                <div
                  id="_desktop_currency_selector"
                  class="
                    currency-selector
                    groups-selector
                    hidden-sm-down
                    currentcy-selector-dropdown
                  "
                >
                  <div
                    class="dropdown-toggle"
                    data-toggle="dropdown"
                    aria-haspopup="true"
                    aria-expanded="false"
                    role="main"
                  >
                    <span class="expand-more">GBP</span>
                  </div>
                  <div class="currency-list dropdown-menu">
                    <div class="currency-list-content text-left">
                      <div class="currency-item current flex-first">
                        <a
                          title="British Pound"
                          rel="nofollow"
                          href="http://demo.bestprestashoptheme.com/savemart/en/?home=&amp;SubmitCurrency=1&amp;id_currency=1"
                          >£ GBP</a
                        >
                      </div>
                      <div class="currency-item">
                        <a
                          title="US Dollar"
                          rel="nofollow"
                          href="http://demo.bestprestashoptheme.com/savemart/en/?home=&amp;SubmitCurrency=1&amp;id_currency=2"
                          >$ USD</a
                        >
                      </div>
                    </div>
                  </div>
                </div>

                <div
                  id="_desktop_language_selector"
                  class="
                    language-selector
                    groups-selector
                    hidden-sm-down
                    language-selector-dropdown
                  "
                >
                  <div
                    class="dropdown-toggle"
                    data-toggle="dropdown"
                    aria-haspopup="true"
                    aria-expanded="false"
                    role="main"
                  >
                    <span class="expand-more"
                      ><img
                        class="img-fluid"
                        src="http://demo.bestprestashoptheme.com/savemart/img/l//1.jpg"
                        alt="English"
                        width="16"
                        height="11"
                    /></span>
                  </div>
                  <div class="language-list dropdown-menu">
                    <div class="language-list-content text-left">
                      <div class="language-item current flex-first">
                        <div class="current">
                          <a
                            href="http://demo.bestprestashoptheme.com/savemart/en/?home="
                          >
                            <img
                              class="img-fluid"
                              src="http://demo.bestprestashoptheme.com/savemart/img/l/1.jpg"
                              alt="English"
                              width="16"
                              height="11"
                            />
                            <span>English</span>
                          </a>
                        </div>
                      </div>
                      <div class="language-item">
                        <div>
                          <a
                            href="http://demo.bestprestashoptheme.com/savemart/fr/?home="
                          >
                            <img
                              class="img-fluid"
                              src="http://demo.bestprestashoptheme.com/savemart/img/l/2.jpg"
                              alt="Français"
                              width="16"
                              height="11"
                            />
                            <span>Français</span>
                          </a>
                        </div>
                      </div>
                      <div class="language-item">
                        <div>
                          <a
                            href="http://demo.bestprestashoptheme.com/savemart/es/?home="
                          >
                            <img
                              class="img-fluid"
                              src="http://demo.bestprestashoptheme.com/savemart/img/l/3.jpg"
                              alt="Español"
                              width="16"
                              height="11"
                            />
                            <span>Español</span>
                          </a>
                        </div>
                      </div>
                      <div class="language-item">
                        <div>
                          <a
                            href="http://demo.bestprestashoptheme.com/savemart/it/?home="
                          >
                            <img
                              class="img-fluid"
                              src="http://demo.bestprestashoptheme.com/savemart/img/l/4.jpg"
                              alt="Italiano"
                              width="16"
                              height="11"
                            />
                            <span>Italiano</span>
                          </a>
                        </div>
                      </div>
                      <div class="language-item">
                        <div>
                          <a
                            href="http://demo.bestprestashoptheme.com/savemart/pl/?home="
                          >
                            <img
                              class="img-fluid"
                              src="http://demo.bestprestashoptheme.com/savemart/img/l/5.jpg"
                              alt="Polski"
                              width="16"
                              height="11"
                            />
                            <span>Polski</span>
                          </a>
                        </div>
                      </div>
                      <div class="language-item">
                        <div>
                          <a
                            href="http://demo.bestprestashoptheme.com/savemart/ar/?home="
                          >
                            <img
                              class="img-fluid"
                              src="http://demo.bestprestashoptheme.com/savemart/img/l/6.jpg"
                              alt="اللغة العربية"
                              width="16"
                              height="11"
                            />
                            <span>اللغة العربية</span>
                          </a>
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

      <div class="header-center hidden-sm-down">
        <div class="container">
          <div class="row d-flex align-items-center">
            <div
              id="_desktop_logo"
              class="
                contentsticky_logo
                d-flex
                align-items-center
                justify-content-start
                col-lg-3 col-md-3
              "
            >
              <a href="http://demo.bestprestashoptheme.com/savemart/">
                <img
                  class="logo img-fluid"
                  src="http://demo.bestprestashoptheme.com/savemart/modules/novthemeconfig/images/logos/logo-1.png"
                  alt="Prestashop_Savemart"
                />
              </a>
            </div>

              <div
                class="
                  col-lg-6 col-md-6
                  header-menu
                  d-flex
                  align-items-center
                  justify-content-start
                "
              >
                <div id="_desktop_top_menu">
                  <nav id="nov-megamenu" class="clearfix">
                    <!-- Brand and toggle get grouped for better mobile display -->
                    <div id="megamenu" class="nov-megamenu clearfix">
                      <ul class="menu level1">
                        <li class="item home-page has-sub">
                          <span class="opener"></span
                          ><a href="?home" title="Home"
                            ><i class="zmdi zmdi-home"></i>Home</a
                          >
                          <div
                            class="dropdown-menu"
                            style="width: 200px; display: none"
                          >
                            <ul class="">
                              <li class="item">
                                <a href="?home=home_1" title="Homepage 1"
                                  >Homepage 1</a
                                >
                              </li>
                              <li class="item">
                                <a href="?home=home_2" title="Homepage 2"
                                  >Homepage 2</a
                                >
                              </li>
                              <li class="item">
                                <a href="?home=home_3" title="Homepage 3"
                                  >Homepage 3</a
                                >
                              </li>
                              <li class="item">
                                <a href="?home=home_4" title="Homepage 4"
                                  >Homepage 4</a
                                >
                              </li>
                              <li class="item">
                                <a href="?home=home_5" title="Homepage 5"
                                  >Homepage 5</a
                                >
                              </li>
                              <li class="item">
                                <a href="?home=home_6" title="Homepage 6"
                                  >Homepage 6</a
                                >
                              </li>
                              <li class="item">
                                <a href="?home=home_7" title="Homepage 7"
                                  >Homepage 7</a
                                >
                              </li>
                              <li class="item">
                                <a href="?home=home_8" title="Homepage 8"
                                  >Homepage 8</a
                                >
                              </li>
                            </ul>
                          </div>
                        </li>

                        <li class="item has-sub">
                          <span class="opener"></span
                          ><a href="#" title="Blog"
                            ><i class="zmdi zmdi-library"></i>Blog</a
                          >
                          <div
                            class="dropdown-menu"
                            style="width: 270px; display: none"
                          >
                            <ul class="">
                              <li class="item">
                                <a
                                  href="/savemart/en/index.php?fc=module&amp;module=smartblog&amp;id_post=14&amp;controller=details"
                                  title="Blog detail"
                                  >Blog detail</a
                                >
                              </li>
                              <li class="item">
                                <a
                                  href="/savemart/blog.html?index.php&amp;cateblog_layout=layout-left-column&amp;cateblog_type=list&amp;cateblog_columns=1"
                                  title="Category Blog ( Left column)"
                                  >Category Blog ( Left column)</a
                                >
                              </li>
                              <li class="item">
                                <a
                                  href="/savemart/blog.html?index.php&amp;cateblog_layout=layout-right-column&amp;cateblog_type=list&amp;cateblog_columns=1"
                                  title="Category Blog ( Right column)"
                                  >Category Blog ( Right column)</a
                                >
                              </li>
                              <li class="item">
                                <a
                                  href="/savemart/blog.html?index.php&amp;cateblog_layout=layout-one-column&amp;cateblog_type=grid&amp;cateblog_columns=1"
                                  title="Category Blog ( One column)"
                                  >Category Blog ( One column)</a
                                >
                              </li>
                              <li class="item">
                                <a
                                  href="/savemart/blog.html?index.php&amp;cateblog_layout=layout-one-column&amp;cateblog_type=grid&amp;cateblog_columns=3"
                                  title="Category Blog ( Grid  column )"
                                  >Category Blog ( Grid column )</a
                                >
                              </li>
                              <li class="item">
                                <a
                                  href="/savemart/blog.html?index.php&amp;cateblog_type=list&amp;cateblog_columns=1&amp;cateblog_layout=layout-one-column"
                                  title="Category Blog List"
                                  >Category Blog List</a
                                >
                              </li>
                            </ul>
                          </div>
                        </li>
                        <li class="item has-sub">
                          <span class="opener"></span
                          ><a href="#" title="Blog"
                            ><i class="zmdi zmdi-library"></i>Pages</a
                          >
                          <div
                            class="dropdown-menu"
                            style="width: 270px; display: none"
                          >
                            <ul class="">
                              <li class="item">
                                <a
                                  href="/savemart/en/index.php?fc=module&amp;module=smartblog&amp;id_post=14&amp;controller=details"
                                  title="Blog detail"
                                  >Blog detail</a
                                >
                              </li>
                              <li class="item">
                                <a
                                  href="/savemart/blog.html?index.php&amp;cateblog_layout=layout-left-column&amp;cateblog_type=list&amp;cateblog_columns=1"
                                  title="Category Blog ( Left column)"
                                  >Category Blog ( Left column)</a
                                >
                              </li>
                              <li class="item">
                                <a
                                  href="/savemart/blog.html?index.php&amp;cateblog_layout=layout-right-column&amp;cateblog_type=list&amp;cateblog_columns=1"
                                  title="Category Blog ( Right column)"
                                  >Category Blog ( Right column)</a
                                >
                              </li>
                              <li class="item">
                                <a
                                  href="/savemart/blog.html?index.php&amp;cateblog_layout=layout-one-column&amp;cateblog_type=grid&amp;cateblog_columns=1"
                                  title="Category Blog ( One column)"
                                  >Category Blog ( One column)</a
                                >
                              </li>
                              <li class="item">
                                <a
                                  href="/savemart/blog.html?index.php&amp;cateblog_layout=layout-one-column&amp;cateblog_type=grid&amp;cateblog_columns=3"
                                  title="Category Blog ( Grid  column )"
                                  >Category Blog ( Grid column )</a
                                >
                              </li>
                              <li class="item">
                                <a
                                  href="/savemart/blog.html?index.php&amp;cateblog_type=list&amp;cateblog_columns=1&amp;cateblog_layout=layout-one-column"
                                  title="Category Blog List"
                                  >Category Blog List</a
                                >
                              </li>
                            </ul>
                          </div>
                        </li>
                        <li class="item has-sub">
                          <span class="opener"></span
                          ><a href="#" title="Blog"
                            ><i class="zmdi zmdi-library"></i>Categories</a
                          >
                          <div
                            class="dropdown-menu"
                            style="width: 270px; display: none"
                          >
                            <ul class="">
                              <li class="item">
                                <a
                                  href="/savemart/en/index.php?fc=module&amp;module=smartblog&amp;id_post=14&amp;controller=details"
                                  title="Blog detail"
                                  >Blog detail</a
                                >
                              </li>
                              <li class="item">
                                <a
                                  href="/savemart/blog.html?index.php&amp;cateblog_layout=layout-left-column&amp;cateblog_type=list&amp;cateblog_columns=1"
                                  title="Category Blog ( Left column)"
                                  >Category Blog ( Left column)</a
                                >
                              </li>
                              <li class="item">
                                <a
                                  href="/savemart/blog.html?index.php&amp;cateblog_layout=layout-right-column&amp;cateblog_type=list&amp;cateblog_columns=1"
                                  title="Category Blog ( Right column)"
                                  >Category Blog ( Right column)</a
                                >
                              </li>
                              <li class="item">
                                <a
                                  href="/savemart/blog.html?index.php&amp;cateblog_layout=layout-one-column&amp;cateblog_type=grid&amp;cateblog_columns=1"
                                  title="Category Blog ( One column)"
                                  >Category Blog ( One column)</a
                                >
                              </li>
                              <li class="item">
                                <a
                                  href="/savemart/blog.html?index.php&amp;cateblog_layout=layout-one-column&amp;cateblog_type=grid&amp;cateblog_columns=3"
                                  title="Category Blog ( Grid  column )"
                                  >Category Blog ( Grid column )</a
                                >
                              </li>
                              <li class="item">
                                <a
                                  href="/savemart/blog.html?index.php&amp;cateblog_type=list&amp;cateblog_columns=1&amp;cateblog_layout=layout-one-column"
                                  title="Category Blog List"
                                  >Category Blog List</a
                                >
                              </li>
                            </ul>
                          </div>
                        </li>
                      </ul>
                    </div>
                  </nav>
                </div>
              </div>
       
            <div
              class="
                contentsticky_group
                col-lg-3 col-md-3
                d-flex
                justify-content-end
                align-items-center
              "
            >
              <div class="header_link_myaccount">
                <a
                  class="login"
                  href="http://demo.bestprestashoptheme.com/savemart/en/my-account"
                  rel="nofollow"
                  title="Log in to your customer account"
                  ><i class="header-icon-account"></i
                ></a>
              </div>
              <div class="header_link_wishlist">
                <a
                  href="http://demo.bestprestashoptheme.com/savemart/en/module/novblockwishlist/mywishlist"
                  title="My Wishlists"
                >
                  <i class="header-icon-wishlist"></i>
                </a>
              </div>
              <div id="_desktop_cart">
                <div
                  class="blockcart cart-preview active"
                  data-refresh-url="//demo.bestprestashoptheme.com/savemart/en/module/ps_shoppingcart/ajax"
                >
                  <div class="header-cart">
                    <div class="cart-left">
                      <div class="shopping-cart">
                        <i class="zmdi zmdi-shopping-cart"></i>
                      </div>
                      <div class="cart-products-count">0</div>
                    </div>
                    <div
                      class="cart-right d-flex flex-column align-self-end ml-13"
                    >
                      <span class="title-cart">Cart</span>
                      <span class="cart-item"> items</span>
                    </div>
                  </div>
                  <div class="cart_block">
                    <div class="cart-block-content">
                      <div class="no-items">No products in the cart</div>
                    </div>
                  </div>
                </div>
              </div>
            </div>
          </div>
        </div>
      </div>

      <div class="header-bottom hidden-sm-down">
        <div class="container">
          <div class="row d-flex align-items-center">
            <div
              class="
                contentsticky_verticalmenu
                verticalmenu-main
                col-md-3 col-lg-3
                d-flex
              "
              data-textshowmore="Show More"
              data-textless="Hide"
              data-desktop_item="3"
            >
              <div
                class="
                  toggle-nav
                  d-flex
                  align-items-center
                  justify-content-start
                "
              >
                <span class="btnov-lines"></span>
                <span>Shop By Categories</span>
                <span class="caret-circle"></span>
              </div>
              <div class="verticalmenu-content has-showmore"></div>
            </div>

            <div
              class="
                col-lg-9 col-md-9
                header-menu
                d-flex
                align-items-center
                justify-content-end
              "
            >
              <div
                class="data-contact d-flex align-items-center hidden-md-down"
              >
                <div class="title-icon">
                  <i class="icon-support icon-address"></i>
                </div>
                <div class="content-data-contact">
                  <div class="support">Call customer services :</div>
                  <div class="phone-support">1234 567 899</div>
                </div>
              </div>
              <div id="_desktop_search" class="contentsticky_search">
                <!-- block seach mobile -->
                <!-- Block search module TOP -->
                <div
                  id="desktop_search_content"
                  data-id_lang="1"
                  data-ajaxsearch="1"
                  data-novadvancedsearch_type="top"
                  data-instantsearch=""
                  data-search_ssl=""
                  data-link_search_ssl="http://demo.bestprestashoptheme.com/savemart/en/search"
                  data-action="http://demo.bestprestashoptheme.com/savemart/en/module/novadvancedsearch/result"
                >
                  <form
                    method="get"
                    action="http://demo.bestprestashoptheme.com/savemart/en/module/novadvancedsearch/result"
                    id="searchbox"
                    class="form-novadvancedsearch"
                  >
                    <input type="hidden" name="fc" value="module" />
                    <input
                      type="hidden"
                      name="module"
                      value="novadvancedsearch"
                    />
                    <input type="hidden" name="controller" value="result" />
                    <input type="hidden" name="orderby" value="position" />
                    <input type="hidden" name="orderway" value="desc" />
                    <input
                      type="hidden"
                      name="id_category"
                      class="id_category"
                      value="0"
                    />
                    <div class="input-group">
                      <input
                        type="text"
                        id="search_query_top"
                        class="
                          search_query
                          ui-autocomplete-input
                          form-control
                          ac_input
                        "
                        name="search_query"
                        value=""
                        placeholder="Search"
                        autocomplete="off"
                      />

                      <div
                        class="input-group-btn nov_category_tree hidden-sm-down"
                      >
                        <button
                          type="button"
                          class="btn dropdown-toggle"
                          data-toggle="dropdown"
                          aria-haspopup="true"
                          value=""
                          aria-expanded="false"
                        >
                          CATEGORIES
                        </button>
                        <ul class="dropdown-menu list-unstyled">
                          <li class="dropdown-item active" data-value="0">
                            <span>All Categories</span>
                          </li>
                          <li class="dropdown-item" data-value="2">
                            <span>Home</span>
                          </li>
                          <ul class="list-unstyled pl-5">
                            <li class="dropdown-item" data-value="3">
                              <span>Computer &amp; Networking</span>
                            </li>
                            <li class="dropdown-item" data-value="10">
                              <span>-- USB</span>
                              <ul class="list-unstyled">
                                <li class="dropdown-item" data-value="11">
                                  <span>---- USB Kingston</span>
                                </li>
                                <li class="dropdown-item" data-value="12">
                                  <span>---- USB Sandisk</span>
                                </li>
                                <li class="dropdown-item" data-value="13">
                                  <span>---- USB Samsung</span>
                                </li>
                              </ul>
                            </li>
                            <li class="dropdown-item" data-value="14">
                              <span>-- Hard Disk</span>
                              <ul class="list-unstyled">
                                <li class="dropdown-item" data-value="19">
                                  <span>---- Hard Disk Drive</span>
                                </li>
                                <li class="dropdown-item" data-value="20">
                                  <span>---- Solid State Drives</span>
                                </li>
                                <li class="dropdown-item" data-value="21">
                                  <span>---- SATA</span>
                                </li>
                              </ul>
                            </li>
                            <li class="dropdown-item" data-value="15">
                              <span>-- Modem WIFI</span>
                            </li>
                            <li class="dropdown-item" data-value="16">
                              <span>-- Keyboard</span>
                              <ul class="list-unstyled">
                                <li class="dropdown-item" data-value="22">
                                  <span>---- Keyboard 1</span>
                                </li>
                                <li class="dropdown-item" data-value="23">
                                  <span>---- Keyboard 2</span>
                                </li>
                              </ul>
                            </li>
                            <li class="dropdown-item" data-value="17">
                              <span>-- Mouse</span>
                            </li>
                            <li class="dropdown-item" data-value="18">
                              <span>-- Monitor</span>
                            </li>
                            <li class="dropdown-item" data-value="6">
                              <span>Laptop &amp; Accessories</span>
                            </li>
                            <li class="dropdown-item" data-value="7">
                              <span>-- Laptop 1</span>
                            </li>
                            <li class="dropdown-item" data-value="8">
                              <span>-- Laptop 2</span>
                            </li>
                            <li class="dropdown-item" data-value="9">
                              <span>Smartphone &amp; Tablet</span>
                            </li>
                            <li class="dropdown-item" data-value="24">
                              <span>-- Apple</span>
                            </li>
                            <li class="dropdown-item" data-value="25">
                              <span>-- Samsung</span>
                            </li>
                            <li class="dropdown-item" data-value="26">
                              <span>-- Motorola</span>
                            </li>
                            <li class="dropdown-item" data-value="27">
                              <span>-- Chargers</span>
                            </li>
                            <li class="dropdown-item" data-value="4">
                              <span>Home Appliance</span>
                            </li>
                            <li class="dropdown-item" data-value="5">
                              <span>Camera &amp; Photo</span>
                            </li>
                            <li class="dropdown-item" data-value="28">
                              <span>-- Camera 1</span>
                            </li>
                            <li class="dropdown-item" data-value="29">
                              <span>-- Camera 2</span>
                            </li>
                            <li class="dropdown-item" data-value="30">
                              <span>-- Photo 1</span>
                            </li>
                            <li class="dropdown-item" data-value="31">
                              <span>-- Photo 2</span>
                            </li>
                            <li class="dropdown-item" data-value="32">
                              <span>Audio</span>
                            </li>
                            <li class="dropdown-item" data-value="33">
                              <span>-- Headphone</span>
                            </li>
                            <li class="dropdown-item" data-value="34">
                              <span>-- Wireless Speaker</span>
                            </li>
                            <li class="dropdown-item" data-value="35">
                              <span>-- Bluetooth Speaker</span>
                            </li>
                            <li class="dropdown-item" data-value="36">
                              <span>-- Mini Speaker</span>
                            </li>
                            <li class="dropdown-item" data-value="37">
                              <span>-- Sound Card</span>
                            </li>
                            <li class="dropdown-item" data-value="38">
                              <span>-- Accessories</span>
                            </li>
                            <li class="dropdown-item" data-value="39">
                              <span>-- Earbuds and In-ear</span>
                            </li>
                          </ul>
                        </ul>
                      </div>

                      <span class="input-group-btn">
                        <button
                          class="btn btn-secondary"
                          type="submit"
                          name="submit_search"
                        >
                          <i class="material-icons">search</i>
                        </button>
                      </span>
                    </div>
                  </form>
                </div>
                <!-- /Block search module TOP -->
              </div>
            </div>
          </div>
        </div>
      </div>
    </header>
  </div>
</template>
<style type="text/css" xml:space="preserve">
li {
  display: inline-block;
}
</style>

