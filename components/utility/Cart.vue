<template>
  <div class="modal right fade" id="cartModal" tabindex="-1" role="dialog" aria-labelledby="exampleModalLabel" aria-hidden="true">
    <div class="modal-dialog modal-lg modal-dialog-centered" role="document">
      <div class="modal-content">
        <div class="modal-header border-bottom-0">
          <h5 class="modal-title" id="exampleModalLabel">
            Your Shopping Cart
          </h5>
          <button type="button" class="close" data-dismiss="modal" aria-label="Close">
            <span aria-hidden="true">&times;</span>
          </button>
        </div>
        <div class="modal-body">
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
                  <img src="https://s3.eu-central-1.amazonaws.com/bootstrapbaymisc/blog/24_days_bootstrap/vans.png" class="img-fluid img-thumbnail" alt="Sheep">
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
</template>

<script>
export default {
  name: 'Cart',
  mounted() {
    $('#cartModal').modal('show');
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
    vertical-align: middle;
    text-align: center;
  }

  .cart-table .qty {
    max-width: 2rem;
  }

  .cart-price {
    margin-left: 1rem;
  }

  .modal-footer {
    padding-top: 0rem;
  }

  /*******************************
  * MODAL AS LEFT/RIGHT SIDEBAR
  * Add "left" or "right" in modal parent div, after class="modal".
  * Get free snippets on bootpen.com
  *******************************/
  .modal.right .modal-dialog {
    position: fixed;
    margin: auto;
    width: 320px;
    height: 100%;
    -webkit-transform: translate3d(0%, 0, 0);
        -ms-transform: translate3d(0%, 0, 0);
        -o-transform: translate3d(0%, 0, 0);
            transform: translate3d(0%, 0, 0);
  }

  .modal.right .modal-content {
    height: 100%;
    overflow-y: auto;
  }

  .modal.right .modal-body {
    padding: 15px 15px 80px;
  }

  /*Right*/
  .modal.right.fade .modal-dialog {
    right: -320px;
    -webkit-transition: opacity 0.3s linear, right 0.3s ease-out;
      -moz-transition: opacity 0.3s linear, right 0.3s ease-out;
        -o-transition: opacity 0.3s linear, right 0.3s ease-out;
            transition: opacity 0.3s linear, right 0.3s ease-out;
  }

  .modal.right.fade.in .modal-dialog {
    right: 0;
  }

  /* ----- MODAL STYLE ----- */
  .cart-modal-footer {
    border-radius: 0;
    border: none;
  }
  /*******************************
  * MODAL AS LEFT/RIGHT SIDEBAR Ends
  *******************************/

</style>
