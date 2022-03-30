<template>
  <div class="row">
    <div v-for="n in 12" :key="n" class="col-md-3">
      <figure class="card card-product-grid">
        <a href="#" class="img-wrap">
          <span class="topbar">
            <span class="badge badge-success"> NEW </span>
          </span>
          <img src="https://d2yz2hr6q3159h.cloudfront.net/marketplace/products/c5374addd1a3d024c3a026199cb8feaf/9127200d-71b8-4935-850c-c874c3c97ba1-1.png">
        </a>
        <figcaption class="info-wrap border-top">
          <a href="#" class="title">Samsung S22 red {{n}}</a>
          <div class="ratring">
            <ul class="rating-stars">
              <li style="width:90%" class="stars-active">
                <i class="fa fa-star"></i><i class="fa fa-star"></i><i class="fa fa-star"></i><i class="fa fa-star"></i><i class="fa fa-star"></i>
              </li>
              <li>
                <i class="fa fa-star"></i><i class="fa fa-star"></i><i class="fa fa-star"></i><i class="fa fa-star"></i><i class="fa fa-star"></i>
              </li>
            </ul>
            <small class="text-muted">34</small>
          </div>
          <div class="price-wrap mt-1">
            <span class="price text-info">৳ 50500</span>
            <small class="price-old" style="text-decoration: line-through; color: #969696 !important;">৳ 60500</small>
          </div> <!-- price-wrap.// -->
          <a href="#" class="mt-2 btn btn-sm btn-outline-primary btn-block">Add to cart <i class="fa fa-shopping-cart"></i></a>
        </figcaption>
      </figure> <!-- card // -->
    </div>
  </div>
</template>

<script>
export default {

}
</script>

<style>

</style>
