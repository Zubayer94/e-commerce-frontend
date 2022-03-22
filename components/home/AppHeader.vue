<template>
  <header class="section-header">
    <section class="header-main border-bottom custom-header">
      <div class="container">
        <div class="row align-items-center">
          <div class="col-lg-2 col-4">
            <div class="brand-wrap">
              <img class="logo" src="~/assets/images/logo.png">
            </div> <!-- brand-wrap.// -->
          </div>
          <div class="col-lg-6 col-sm-12">
            <!-- search-wrap .end// -->
            <form action="#" class="search">
              <div class="input-group w-100">
                <select class="custom-select"  name="category_name">
                  <option value="all">All type</option>
                  <option value="buy">Buy</option>
                  <option value="sell">Sell</option>
                  <option value="swap">Swap</option>
                </select>
                  <input type="text" class="form-control" style="width:50%;" placeholder="Search">
                  <div class="input-group-append">
                    <button class="btn btn-primary" type="submit">
                      <i class="fa fa-search"></i>
                    </button>
                  </div>
                </div>
            </form>
            <!-- search-wrap .end// -->
          </div> <!-- col.// -->
          <div class="col-lg-4 col-sm-6 col-8">
            <div class="widgets-wrap float-md-right">

              <div class="widget-header  mr-3 dropdown " >
                <a href="#" @select="handleCartDropdown" class="icon icon-sm rounded-circle border caret-off dropdown-toggle" id="dropdownMenuButton" data-toggle="dropdown" aria-haspopup="true" aria-expanded="false" > <!-- can also handle by mouseenter -->
                  <i class="fa fa-shopping-cart"></i>
                </a>
                <span class="badge badge-pill badge-danger notify">0</span>

                <div class="dropdown-menu cart-menu" aria-labelledby="dropdownMenuButton" style="width: 350px;">
                  <!-- <p>No products</p> -->

                  <!-- <div class="modal-content"> -->
                    <div class="modal-header border-bottom-0">
                      <h6 class="modal-title" id="exampleModalLabel">
                        <i class="fa-solid fa-cart-shopping text-dark"></i> 6 Items
                      </h6>
                      <button type="button" class="close" @click="closeDropdown">
                        <span aria-hidden="true">&times;</span>
                      </button>
                    </div>
                    <div class="modal-body p-2 cartModal-body">
                      <table class="cart-table">
                        <tbody>
                          <tr v-for="n in 5" :key="n" class="p-0 mb-2">
                            <td class="col-sm-1 col-md-1 col-1 px-1 text-center">
                              <button class="increase btn btn-sm">
                                  <i class="fa-solid fa-square-plus text-warning"></i>
                              </button>
                              <p class="cart-quantity-text m-0">1</p>
                              <button class="decrease btn btn-sm">
                                  <i class="fa-solid fa-square-minus text-warning"></i>
                              </button>
                            </td>
                            <td class="col-sm-8 col-md-7 col-7 px-1 mb-2">
                              <div class="row">
                                <div class="col-4 p-1 cart-product-image w-30" >
                                  <img src="https://d2yz2hr6q3159h.cloudfront.net/marketplace/products/b8a03c5c15fcfa8dae0b03351eb1742f/pre-owned-iphone-12-pro-max-256gb-pacific-blue-4850.png" class="img-fluid mt-1" alt="Sheep" width="60px">
                                </div>

                                <div class="col-8 p-1 cart-product-body w-70" >
                                  <p class="product-name m-0">
                                      <a href="#">iPhone 12 Pro Max 256GB Pacific Blue{{n}}</a>
                                  </p>
                                  <p class="product-price">
                                      <TakaLogo :height="15" :width="15" /><a href="#">
                                          <span style="text-decoration: line-through; color: rgb(36, 36, 36) !important;">155000</span> <span class="text-success"> <b>৳ 94999</b></span> / Piece
                                      </a>
                                  </p>
                                </div>
                              </div>
                            </td>
                            <td class="col-sm-1 col-md-3 col-3 px-1 text-center">
                              <TakaLogo :height="15" :width="15" />890000
                            </td>
                            <td class="col-sm-1 col-md-3 col-3 px-1 text-center del-cart-button">
                              <button class="btn btn-sm">
                                <i class="fa fa-trash-o text-danger"></i>
                              </button>
                            </td>
                          </tr>
                        </tbody>
                      </table>
                      <!-- <div class="d-flex justify-content-end">
                        <h5>Total: <span class="cart-price text-success">৳ 89</span></h5>
                      </div> -->
                    </div>
                    <div class="modal-footer cart-modal-footer border-top-0 d-flex justify-content-between">
                      <h5>Total: <span class="cart-price text-success">৳ 89</span></h5>
                      <!-- <button type="button" class="btn btn-secondary" @click="closeDropdown">Close</button> -->
                      <button type="button" class="btn btn-success">Checkout</button>
                    </div>
                  <!-- </div> -->
                </div>
              </div>

              <div class="widget-header icontext">
                <a href="#" class="icon icon-sm rounded-circle border"><i class="fa fa-user"></i></a>
                <div class="text">
                  <span class="text-muted">Welcome!</span>
                  <div>
                    <a href="#">Sign in</a> |
                    <a href="#"> Register</a>
                  </div>
                </div>
              </div>
            </div> <!-- widgets-wrap.// -->
          </div> <!-- col.// -->
        </div> <!-- row.// -->
      </div> <!-- container.// -->
    </section> <!-- header-main .// -->
  </header> <!-- section-header.// -->
</template>

<script>
import TakaLogo from '../custom/TakaLogo.vue';
export default {
  components: { TakaLogo },
  methods: {
    handleCartDropdown() {
      $('.dropdown-toggle').dropdown('show')
    },
    closeDropdown() {
      $('.dropdown-toggle').dropdown('hide')
    },
  },
}
</script>

<style>
  .cart-table .thead td, .cart-table .thead th {
    border: 0;
    color: #666;
    font-size: 0.8rem;
  }

  .cart-table td, .cart-table th {
    border: 0;
    vertical-align: middle;
    text-align: center;
  }

  .cart-price {
    margin-left: 1rem;
  }

  .cartModal-body {
    height: 300px;
    overflow-y: scroll;
  }

  .cart-product-body p{
    font-size: 12px;
    font-weight: 500;
    font-stretch: normal;
    font-style: normal;
    line-height: 1.33;
    letter-spacing: normal;
    text-align: left;
    transition: all .4s ease;
  }
  .cart-product-body a:hover{
    color: #007bff;
  }
  /* manage cart width from 375px */
  @media screen and (max-width: 375px) {
    .cart-menu {
      width: 320px !important;
    }
  }
</style>

