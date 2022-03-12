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
              <div class="widget-header  mr-3">
                <a href="#" @click="openModal" class="icon icon-sm rounded-circle border"><i class="fa fa-shopping-cart"></i></a>
                <span class="badge badge-pill badge-danger notify">0</span>
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

    <!-- Modal -->
    <!-- <div class="modal fade cartModal" id="cartModal" tabindex="-1" role="dialog" aria-labelledby="exampleModalLabel" aria-hidden="true" data-keyboard="false" data-backdrop="static">
      <div class="modal-dialog modal-dialog-centered cartModal-dialog" role="document">
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
            <table class="table cart-table">
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
    </div> -->
    <!-- modal -->

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
            <table class="table cart-table">
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
export default {
  methods: {
    openModal() {
    $('#supportModal').modal('show');
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

  .cart-table .qty {
    max-width: 2rem;
  }

  .cart-price {
    margin-left: 1rem;
  }

  .cart-modal-footer {
    padding-top: 0rem;
  }

  /*******************************
  * MODAL AS RIGHT SIDEBAR
  *******************************/
  /* .cartModal .cartModal-dialog {
    position:fixed;
    bottom: 50px;
    right: 30px;
    width: 70%;
    margin:0;
  }
  .cartModal-dialog{
    overflow-y: initial !important
  }
  .cartModal-body{
      max-height: calc(50vh - 100px);
      overflow-y: auto;
  } */

  .supportModal .supportModal-dialog {
    position: fixed;
    top: 15%;
    right: 0px;
    width: 70%;
    margin: 0;
  }
  .supportModal-dialog{
    overflow-y: initial !important
  }
  .supportModal-body{
      max-height: calc(50vh - 100px);
      overflow-y: auto;
  }
  /*******************************
  * MODAL AS RIGHT SIDEBAR Ends
  *******************************/

</style>

