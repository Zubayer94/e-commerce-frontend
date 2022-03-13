<template>
  <header class="section-header">
    <section class="header-main border-bottom">
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

              <div class="widget-header  mr-3 dropdown" >
                <a href="#" @mouseenter="handleCartDropdown" class="icon icon-sm rounded-circle border caret-off dropdown-toggle" id="dropdownMenuButton" data-toggle="dropdown" aria-haspopup="true" aria-expanded="false" >
                  <i class="fa fa-shopping-cart"></i>
                </a>
                <span class="badge badge-pill badge-danger notify">0</span>

                <div class="dropdown-menu" aria-labelledby="dropdownMenuButton">
                  <!-- <p>No products</p> -->

                  <!-- <div class="modal-content"> -->
                    <div class="modal-header border-bottom-0">
                      <h5 class="modal-title" id="exampleModalLabel">
                        Your Shopping Cart
                      </h5>
                      <button type="button" class="close" data-dismiss="modal" aria-label="Close">
                        <span aria-hidden="true">&times;</span>
                      </button>
                    </div>
                    <div class="modal-body cartModal-body">
                      <table class="table table-responsive cart-table">
                        <!-- <thead>
                          <tr>
                            <th scope="col">Qty</th>
                            <th scope="col">Product</th>
                            <th scope="col">Total</th>
                            <th scope="col">Actions</th>
                          </tr>
                        </thead> -->
                        <tbody>
                          <tr>
                            <td class="col-sm-1 col-md-1 col-1 text-center">
                              <button class="increase btn btn-sm">
                                  <i class="fa-solid fa-square-plus text-warning"></i>
                              </button>
                              <p class="cart-quantity-text m-0">1</p>
                              <button class="decrease btn btn-sm">
                                  <i class="fa-solid fa-square-minus text-warning"></i>
                              </button>
                            </td>
                            <td class="col-sm-8 col-md-7 col-7 w-25">
                              <div class="cart-product-image" >
                                <img src="https://s3.eu-central-1.amazonaws.com/bootstrapbaymisc/blog/24_days_bootstrap/vans.png" class="img-fluid img-thumbnail" alt="Sheep" width="60px" >
                              </div>
                              <div class="cart-product-body" >
                                <p class="product-name">
                                    <a href="#">iPhone 12 Pro Max 256GB Pacific Blue (Certified Pre-owned)</a>
                                </p>
                                <p class="product-price">
                                    <TakaLogo :height="15" :width="15" /><a href="#">
                                        <span style="text-decoration: line-through; color: rgb(36, 36, 36) !important;">155000</span> <!---->
                                        <span>94999</span> / Piece
                                    </a>
                                </p>
                              </div>
                            </td>
                            <td class="col-sm-1 col-md-3 col-3 text-center w-75">
                              <TakaLogo :height="15" :width="15" />89
                            </td>
                            <td class="col-sm-1 col-md-3 col-3 text-center">
                              <button class="btn btn-sm">
                                <i class="fa fa-trash-o text-dark"></i>
                              </button>
                            </td>
                          </tr>
                        </tbody>
                      </table>
                      <div class="d-flex justify-content-end">
                        <h5>Total: <span class="cart-price text-success">৳ 89</span></h5>
                      </div>
                    </div>
                    <div class="modal-footer cart-modal-footer border-top-0 d-flex justify-content-between">
                      <button type="button" class="btn btn-secondary" data-dismiss="modal">Close</button>
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

    <div class="modal fade supportModal" id="supportModal" tabindex="-1" role="dialog" aria-labelledby="supportModalLabel" aria-hidden="true" data-keyboard="false" data-backdrop="static">
      <div class="modal-dialog supportModal-dialog" role="document">
        <div class="modal-content">
          <div class="modal-header border-bottom-0">
            <h5 class="modal-title" id="exampleModalLabel">
              Your Shopping Cart
            </h5>
            <button type="button" class="close" data-dismiss="modal" aria-label="Close">
              <span aria-hidden="true">&times;</span>
            </button>
          </div>
          <div class="modal-body cartModal-body">
            <table class="table table-responsive cart-table">
              <thead>
                <tr>
                  <th scope="col"></th>
                  <th scope="col">Product</th>
                  <th scope="col">Price</th>
                  <th scope="col">Qty</th>
                  <th scope="col">Total</th>
                  <th scope="col">Actions</th>
                </tr>
              </thead>
              <tbody>
                <tr>
                  <td class="w-25">
                    <img src="https://s3.eu-central-1.amazonaws.com/bootstrapbaymisc/blog/24_days_bootstrap/vans.png"
                      class="img-fluid img-thumbnail" alt="Sheep">
                  </td>
                  <td>Vans Sk8-Hi MTE Shoes</td>
                  <td>89$</td>
                  <td class="qty"><input type="text" class="form-control" id="input1" value="2"></td>
                  <td>178$</td>
                  <td>
                    <a href="#" class="btn btn-danger btn-sm">
                      <i class="fa fa-times"></i>
                    </a>
                  </td>
                </tr>
              </tbody>
            </table>
            <div class="d-flex justify-content-end">
              <h5>Total: <span class="cart-price text-success">89$</span></h5>
            </div>
          </div>
          <div class="modal-footer cart-modal-footer border-top-0 d-flex justify-content-between">
            <button type="button" class="btn btn-secondary" data-dismiss="modal">Close</button>
            <button type="button" class="btn btn-success">Checkout</button>
          </div>
        </div>
      </div>
    </div>

  </header> <!-- section-header.// -->
</template>

<script>
import TakaLogo from '../custom/TakaLogo.vue';
export default {
  components: { TakaLogo },
  methods: {
    handleCartDropdown() {
      console.log('hovered');
    // $('#supportModal').modal('show');
      $('.dropdown-toggle').dropdown('toggle')
    }
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

  /* remove dropdown arrow logo */
  .caret-off::before {
    display: none;
  }
  .caret-off::after {
      display: none;
  }
</style>

