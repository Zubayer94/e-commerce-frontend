<template>
  <section class="section-main bg padding-y py-2">
    <div class="container">
      <div class="row">
        <div class="col-md-12">
          <!-- <article class="banner-wrap">
            <img src="~/assets/ui/images/banners/banner.jpg" class="w-100 rounded">
          </article> -->

          <article>
            <!-- ================== COMPONENT SLIDER  BOOTSTRAP  ==================  -->
            <div id="carousel1_indicator" class="carousel slide" data-ride="carousel">
              <ol class="carousel-indicators">
                <li data-target="#carousel1_indicator" data-slide-to="0" class="active"></li>
                <li data-target="#carousel1_indicator" data-slide-to="1"></li>
                <li data-target="#carousel1_indicator" data-slide-to="2"></li>
                <li data-target="#carousel1_indicator" data-slide-to="3"></li>
              </ol>
              <div class="carousel-inner">
                <div class="carousel-item active">
                  <img class="d-block w-100" src="~/assets/images/buyBanner1.jpg" alt="First slide">
                </div>
                <div class="carousel-item">
                  <img class="d-block w-100" src="~/assets/images/buyBanner2.jpg" alt="Second slide">
                </div>
                <div class="carousel-item">
                  <img class="d-block w-100" src="~/assets/images/buyBanner3.png" alt="Third slide">
                </div>
                <div class="carousel-item">
                  <img class="d-block w-100" src="~/assets/images/buyBanner4.png" alt="Third slide">
                </div>
              </div>
              <a class="carousel-control-prev" href="#carousel1_indicator" role="button" data-slide="prev">
                <span class="carousel-control-prev-icon" aria-hidden="true"></span>
                <span class="sr-only">Previous</span>
              </a>
              <a class="carousel-control-next" href="#carousel1_indicator" role="button" data-slide="next">
                <span class="carousel-control-next-icon" aria-hidden="true"></span>
                <span class="sr-only">Next</span>
              </a>
            </div>
            <!-- ==================  COMPONENT SLIDER BOOTSTRAP end.// ==================  .// -->
          </article> <!-- col.// -->
        </div> <!-- col.// -->
      </div> <!-- row.// -->
    </div> <!-- container //  -->
  </section>
</template>

<script>
export default {

}
</script>

<style>

</style>
