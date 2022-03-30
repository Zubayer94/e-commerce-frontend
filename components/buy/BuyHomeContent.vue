<template>
  <section class="section-name padding-y-sm">
    <div class="container">
      <!-- ============== Hot deals SLIDER ITEMS SLICK  ============= -->
      <div class="popular-product">
        <header class="section-heading my-3">
          <a href="#" class="btn btn-outline-primary float-right">See all</a>
          <h4 class="section-title">Hot Deals</h4>
        </header><!-- sect-heading -->
        <div class="slider-items-slick row" data-slick='{"slidesToShow": 4, "slidesToScroll": 1}'>
          <div v-for="n in 8" :key="n" class="col-md-3">
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
      </div>
      <!-- ============== Hot deals SLIDER ITEMS SLICK .end // ============= -->

      <!-- ============== Smartphone SLIDER ITEMS SLICK  ============= -->
      <div class="popular-product">
        <header class="section-heading my-3">
          <a href="#" class="btn btn-outline-primary float-right">See all</a>
          <h4 class="section-title">Smartphone</h4>
        </header><!-- sect-heading -->
        <div class="slider-items-slick row" data-slick='{"slidesToShow": 4, "slidesToScroll": 1}'>
          <div v-for="n in 8" :key="n" class="col-md-3">
            <figure class="card card-product-grid">
              <a href="#" class="img-wrap">
                <span class="topbar">
                  <span class="badge badge-success"> NEW </span>
                </span>
                <img src="https://d2yz2hr6q3159h.cloudfront.net/marketplace/products/c5374addd1a3d024c3a026199cb8feaf/9127200d-71b8-4935-850c-c874c3c97ba1-1.png">
              </a>
              <figcaption class="info-wrap border-top">
                <a href="#" class="title">Samsung S22 Red {{n}}</a>
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
      </div>
      <!-- ============== Smartphone SLIDER ITEMS SLICK .end // ============= -->

      <!-- ============== Laptop SLIDER ITEMS SLICK  ============= -->
      <div class="popular-product">
        <header class="section-heading my-3">
          <a href="#" class="btn btn-outline-primary float-right">See all</a>
          <h4 class="section-title">Laptop</h4>
        </header><!-- sect-heading -->
        <div class="slider-items-slick row" data-slick='{"slidesToShow": 4, "slidesToScroll": 1}'>
          <div v-for="n in 8" :key="n" class="col-md-3">
            <figure class="card card-product-grid">
              <a href="#" class="img-wrap">
                <span class="topbar">
                  <span class="badge badge-success"> NEW </span>
                </span>
                <img src="https://d2yz2hr6q3159h.cloudfront.net/marketplace/products/8e3308c853e47411c761429193511819/3ce91063-b796-4254-966b-4281143090ef-0271b471-0cad-41be-b188-538304fc8f13-1.png">
              </a>
              <figcaption class="info-wrap border-top">
                <a href="#" class="title">Samsung S22 Red {{n}}</a>
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
      </div>
      <!-- ============== Laptop SLIDER ITEMS SLICK .end // ============= -->

      <!-- ============== Motorcycle SLIDER ITEMS SLICK  ============= -->
      <div class="popular-product">
        <header class="section-heading my-3">
          <a href="#" class="btn btn-outline-primary float-right">See all</a>
          <h4 class="section-title">Motorcycle</h4>
        </header><!-- sect-heading -->
        <div class="slider-items-slick row" data-slick='{"slidesToShow": 4, "slidesToScroll": 1}'>
          <div v-for="n in 8" :key="n" class="col-md-3">
            <figure class="card card-product-grid">
              <a href="#" class="img-wrap">
                <span class="topbar">
                  <span class="badge badge-success"> NEW </span>
                </span>
                <img src="https://d2yz2hr6q3159h.cloudfront.net/marketplace/products/ba530cdf0a884348613f2aaa3a5ba5e8/bajaj-avenger-160-street-abs-11333.jpg">
              </a>
              <figcaption class="info-wrap border-top">
                <a href="#" class="title">Samsung S22 Red {{n}}</a>
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
      </div>
      <!-- ============== Motorcycle SLIDER ITEMS SLICK .end // ============= -->
    </div><!-- container // -->
  </section>
</template>

<script>
export default {
  mounted() {
    /////////////////  items slider. /plugins/slickslider/
    // check if element exists
    if ($('.slider-items-slick').length > 0) {
      $('.slider-items-slick').slick({
          autoplay: true,
          arrows: true,
          infinite: true,
          swipeToSlide: true,
          slidesToShow: 4,
          dots: false,
          slidesToScroll: 2,
          prevArrow: '<button type="button" class="slick-prev"><i class="fa-solid fa-angle-left"></i></button>',
          nextArrow: '<button type="button" class="slick-next"><i class="fa-solid fa-angle-right"></i></button>',
          responsive: [
              {
                  breakpoint: 768,
                  settings: {
                      slidesToShow: 2
                  }
              },
              {
                  breakpoint: 640,
                  settings: {
                      slidesToShow: 1
                  }
              }
          ]
      });
    }
    // end if
  },
}
</script>

<style>

</style>
