<template>
  <div>
    <!-- ========================= SECTION INTRO ========================= -->
    <section class="section-intro padding-y-sm py-2">
      <div class="container">
        <div class="intro-banner-wrap">
          <img src="https://d2yz2hr6q3159h.cloudfront.net/mp-category/03afdbd66e7929b125f8597834fa83a4/banner/laptop.png" class="img-fluid">
        </div>
      </div> <!-- container //  -->
    </section>
    <!-- ========================= SECTION INTRO END// ========================= -->

    <!-- ========================= SECTION CONTENT ========================= -->
    <section class="section-content padding-y py-2">
      <div class="container">
        <div class="row">
          <aside class="col-md-3">
            <div class="card">
              <article class="filter-group">
                <header class="card-header">
                  <a href="#" data-toggle="collapse" data-target="#collapse_1" aria-expanded="true" class="">
                    <i class="icon-control fa fa-chevron-down"></i>
                    <h6 class="title">Ctegory</h6>
                  </a>
                </header>
                <div class="filter-content collapse show" id="collapse_1" style="">
                  <div class="card-body">
                    <TreeCategoryFilterMenu
                      v-for="category in categoryTree"
                      :key="category.id"
                      :category="category"
                    />
                  </div> <!-- card-body.// -->
                </div>
              </article> <!-- filter-group  .// -->

              <article class="filter-group">
                <header class="card-header">
                  <a href="#" data-toggle="collapse" data-target="#collapse_1" aria-expanded="true" class="">
                    <i class="icon-control fa fa-chevron-down"></i>
                    <h6 class="title">Product type</h6>
                  </a>
                </header>
                <div class="filter-content collapse show" id="collapse_1" style="">
                  <div class="card-body">
                    <form class="pb-3">
                      <div class="input-group">
                        <input type="text" class="form-control" placeholder="Search">
                        <div class="input-group-append">
                          <button class="btn btn-light" type="button"><i class="fa fa-search"></i></button>
                        </div>
                      </div>
                    </form>

                    <ul class="list-menu">
                      <li><a href="#">People </a></li>
                      <li><a href="#">Watches </a></li>
                      <li><a href="#">Cinema </a></li>
                      <li><a href="#">Clothes </a></li>
                      <li><a href="#">Home items </a></li>
                      <li><a href="#">Animals</a></li>
                      <li><a href="#">People </a></li>
                    </ul>
                  </div> <!-- card-body.// -->
                </div>
              </article> <!-- filter-group  .// -->

              <article class="filter-group">
                <header class="card-header">
                  <a href="#" data-toggle="collapse" data-target="#collapse_2" aria-expanded="true" class="">
                    <i class="icon-control fa fa-chevron-down"></i>
                    <h6 class="title">Brands </h6>
                  </a>
                </header>
                <div class="filter-content collapse show" id="collapse_2" style="">
                  <div class="card-body">
                    <label class="custom-control custom-checkbox">
                      <input type="checkbox" checked="" class="custom-control-input">
                      <div class="custom-control-label">Mercedes
                        <b class="badge badge-pill badge-light float-right">120</b>
                      </div>
                    </label>
                    <label class="custom-control custom-checkbox">
                      <input type="checkbox" checked="" class="custom-control-input">
                      <div class="custom-control-label">Toyota
                        <b class="badge badge-pill badge-light float-right">15</b>
                      </div>
                    </label>
                    <label class="custom-control custom-checkbox">
                      <input type="checkbox" checked="" class="custom-control-input">
                      <div class="custom-control-label">Mitsubishi
                        <b class="badge badge-pill badge-light float-right">35</b>
                      </div>
                    </label>
                    <label class="custom-control custom-checkbox">
                      <input type="checkbox" checked="" class="custom-control-input">
                      <div class="custom-control-label">Nissan
                        <b class="badge badge-pill badge-light float-right">89</b>
                      </div>
                    </label>
                    <label class="custom-control custom-checkbox">
                      <input type="checkbox" class="custom-control-input">
                      <div class="custom-control-label">Honda
                        <b class="badge badge-pill badge-light float-right">30</b>
                      </div>
                    </label>
                  </div> <!-- card-body.// -->
                </div>
              </article> <!-- filter-group .// -->

              <article class="filter-group">
                <header class="card-header">
                  <a href="#" data-toggle="collapse" data-target="#collapse_3" aria-expanded="true" class="">
                    <i class="icon-control fa fa-chevron-down"></i>
                    <h6 class="title">Price range </h6>
                  </a>
                </header>
                <div class="filter-content collapse show" id="collapse_3" style="">
                  <div class="card-body">
                    <input type="range" class="custom-range" min="0" max="100" name="">
                    <div class="form-row">
                      <div class="form-group col-md-6">
                        <label>Min</label>
                        <input class="form-control" placeholder="$0" type="number">
                      </div>
                      <div class="form-group text-right col-md-6">
                        <label>Max</label>
                        <input class="form-control" placeholder="$1,0000" type="number">
                      </div>
                    </div> <!-- form-row.// -->
                    <button class="btn btn-block btn-primary">Apply</button>
                  </div><!-- card-body.// -->
                </div>
              </article> <!-- filter-group .// -->

              <article class="filter-group">
                <header class="card-header">
                  <a href="#" data-toggle="collapse" data-target="#collapse_4" aria-expanded="true" class="">
                    <i class="icon-control fa fa-chevron-down"></i>
                    <h6 class="title">Sizes </h6>
                  </a>
                </header>
                <div class="filter-content collapse show" id="collapse_4" style="">
                  <div class="card-body">
                    <label class="checkbox-btn">
                      <input type="checkbox">
                      <span class="btn btn-light"> XS </span>
                    </label>

                    <label class="checkbox-btn">
                      <input type="checkbox">
                      <span class="btn btn-light"> SM </span>
                    </label>

                    <label class="checkbox-btn">
                      <input type="checkbox">
                      <span class="btn btn-light"> LG </span>
                    </label>

                    <label class="checkbox-btn">
                      <input type="checkbox">
                      <span class="btn btn-light"> XXL </span>
                    </label>
                  </div><!-- card-body.// -->
                </div>
              </article> <!-- filter-group .// -->

              <article class="filter-group">
                <header class="card-header">
                  <a href="#" data-toggle="collapse" data-target="#collapse_5" aria-expanded="false" class="">
                    <i class="icon-control fa fa-chevron-down"></i>
                    <h6 class="title">More filter </h6>
                  </a>
                </header>
                <div class="filter-content collapse in" id="collapse_5" style="">
                  <div class="card-body">
                    <label class="custom-control custom-radio">
                      <input type="radio" name="myfilter_radio" checked="" class="custom-control-input">
                      <div class="custom-control-label">Any condition</div>
                    </label>

                    <label class="custom-control custom-radio">
                      <input type="radio" name="myfilter_radio" class="custom-control-input">
                      <div class="custom-control-label">Brand new </div>
                    </label>

                    <label class="custom-control custom-radio">
                      <input type="radio" name="myfilter_radio" class="custom-control-input">
                      <div class="custom-control-label">Used items</div>
                    </label>

                    <label class="custom-control custom-radio">
                      <input type="radio" name="myfilter_radio" class="custom-control-input">
                      <div class="custom-control-label">Very old</div>
                    </label>
                  </div><!-- card-body.// -->
                </div>
              </article> <!-- filter-group .// -->
            </div> <!-- card.// -->
          </aside> <!-- col.// -->

          <main class="col-md-9">
            <header class="border-bottom mb-4 pb-3">
              <div class="form-inline">
                <span class="mr-md-auto">32 Items found </span>
                <select class="mr-2 form-control">
                  <option>Latest items</option>
                  <option>Trending</option>
                  <option>Most Popular</option>
                  <option>Cheapest</option>
                </select>
                <div class="btn-group">
                  <button @click="isSmallGrid(true)" class="btn btn-outline-secondary" :class="smallGrid ? 'active' : ''" data-toggle="tooltip" title="List view">
                    <i class="fa fa-bars"></i>
                  </button>
                  <button @click="isSmallGrid(false)" class="btn  btn-outline-secondary" :class="!smallGrid ? 'active' : ''" data-toggle="tooltip" title="Grid view">
                    <i class="fa fa-th"></i>
                  </button>
                </div>
              </div>
            </header><!-- sect-heading -->

            <template v-if="smallGrid">
              <BuyProductListGrid />
            </template>
            <template v-else >
              <BuyProducLargetListGrid />
            </template>

            <nav class="mt-3" aria-label="Page navigation sample">
              <ul class="pagination float-right">
                <li class="page-item disabled"><a class="page-link" href="#">Previous</a></li>
                <li class="page-item active"><a class="page-link" href="#">1</a></li>
                <li class="page-item"><a class="page-link" href="#">2</a></li>
                <li class="page-item"><a class="page-link" href="#">3</a></li>
                <li class="page-item"><a class="page-link" href="#">Next</a></li>
              </ul>
            </nav>

          </main> <!-- col.// -->

        </div>

      </div> <!-- container .//  -->
    </section>
    <!-- ========================= SECTION CONTENT END// ========================= -->
  </div>
</template>

<script>
import BuyProducLargetListGrid from '../../../components/buy/BuyProducLargetListGrid.vue'
import BuyProductListGrid from '../../../components/buy/BuyProductListGrid.vue'
import TreeCategoryFilterMenu from '../../../components/buy/TreeCategoryFilterMenu.vue'
export default {
  components: { BuyProductListGrid, BuyProducLargetListGrid, TreeCategoryFilterMenu },
  layout: 'buy',
  data() {
    return {
      smallGrid: true,
      categoryTree: [
        {
          "id": 4,
          "title": "Phones & Accessories",
          "slug": "phones-accessories",
          "child": [
            {
              "id": 31,
              "title": "Smartphone",
              "slug": "smartphone",
              "child": [
                  {
                      "id": 5,
                      "title": "Samsung",
                      "slug": "samsung",
                  },
                  {
                      "id": 33,
                      "title": "Xiaomi",
                      "slug": "xiaomi",
                  },
                  {
                      "id": 34,
                      "title": "Huawei",
                      "slug": "huawei",
                  },
                  {
                      "id": 35,
                      "title": "OnePlus",
                      "slug": "oneplus",
                  },
                  {
                      "id": 36,
                      "title": "Oppo",
                      "slug": "oppo",
                  },
                  {
                      "id": 37,
                      "title": "Realme",
                      "slug": "realme",
                  },
                  {
                      "id": 38,
                      "title": "Vivo",
                      "slug": "vivo",
                  },
                  {
                      "id": 40,
                      "title": "Apple",
                      "slug": "apple",
                  },
                  {
                      "id": 54,
                      "title": "Google",
                      "slug": "google",
                  },
                  {
                      "id": 55,
                      "title": "Nokia",
                      "slug": "nokia",
                  },
                  {
                      "id": 56,
                      "title": "Motorola",
                      "slug": "motorola",
                  },
                  {
                      "id": 57,
                      "title": "Asus",
                      "slug": "asus",
                  },
                  {
                      "id": 58,
                      "title": "LG",
                      "slug": "lg",
                  },
                  {
                      "id": 124,
                      "title": "Honor",
                      "slug": "honor",
                  }
              ]
            },
            {
                "id": 32,
                "title": "Accessories",
                "slug": "accessories",
            }
          ]
        },
        {
          "id": 121,
          "title": "Motorcycle",
          "slug": "motorcycle",
          "child": [
            {
                "id": 122,
                "title": "Motorbikes",
                "slug": "motorbikes",
            },
            {
                "id": 123,
                "title": "Scooter",
                "slug": "scooter",
            },
            {
                "id": 126,
                "title": "E-bikes",
                "slug": "e-bikes",
            }
          ]
        },
        {
          "id": 106,
          "title": "Automobiles",
          "slug": "automobiles",
          "child": [
            {
                "id": 107,
                "title": "Sedan",
                "slug": "sedan",
            },
            {
                "id": 111,
                "title": "SUV",
                "slug": "suv",
            },
            {
                "id": 131,
                "title": "Hatchback",
                "slug": "hatchback",
            }
          ]
        },
        {
          "id": 63,
          "title": "Laptop",
          "slug": "laptop",
          "child": [
            {
                "id": 70,
                "title": "Acer",
                "slug": "acer",
            },
            {
                "id": 71,
                "title": "Asus Laptop",
                "slug": "asus-laptop",
            },
            {
                "id": 72,
                "title": "Dell",
                "slug": "dell",
            },
            {
                "id": 73,
                "title": "HP",
                "slug": "hp",
            },
            {
                "id": 74,
                "title": "Lenovo",
                "slug": "lenovo",
            },
            {
                "id": 75,
                "title": "Surface",
                "slug": "surface",
            },
            {
                "id": 76,
                "title": "Razer",
                "slug": "razer",
            },
            {
                "id": 77,
                "title": "MacBook",
                "slug": "macbook",
            },
            {
                "id": 146,
                "title": "MSI",
                "slug": "msi",
            },
            {
                "id": 208,
                "title": "iMac",
                "slug": "imac",
            },
            {
                "id": 209,
                "title": "NEC",
                "slug": "nec",
            },
            {
                "id": 210,
                "title": "Fujitsu",
                "slug": "fujitsu",
            },
            {
                "id": 213,
                "title": "Panasonic",
                "slug": "panasonic",
            }
          ]
        },
        {
          "id": 79,
          "title": "Repair & Servicing",
          "slug": "repair-servicing",
          "child": [
              {
                "id": 80,
                "title": "Smartphone Servicing",
                "slug": "smartphone-servicing",
                "child": [
                  {
                      "id": 84,
                      "title": "Smartphone LCD",
                      "slug": "smartphone-lcd",
                  },
                  {
                      "id": 85,
                      "title": "Smartphone Motherboard",
                      "slug": "smartphone-motherboard",
                  },
                  {
                      "id": 94,
                      "title": "Smartphone Battery",
                      "slug": "smartphone-battery",
                  }
                ]
              }
          ]
        },
        {
          "id": 155,
          "title": "Furniture",
          "slug": "furniture",
          "child": [
            {
                "id": 156,
                "title": "Bedroom",
                "slug": "bedroom",
            },
            {
                "id": 157,
                "title": "Living Room",
                "slug": "living-room",
            },
            {
                "id": 158,
                "title": "Dinning Room",
                "slug": "dinning-room",
            },
            {
                "id": 160,
                "title": "Office",
                "slug": "office",
            }
          ]
        },
        {
          "id": 211,
          "title": "Merchandise",
          "slug": "merchandise",
          "child": [
            {
                "id": 212,
                "title": "Chattogram Challengers",
                "slug": "chattogram-challengers",
            }
          ]
        }
      ]
    }
  },
  methods: {
    isSmallGrid(data){
      this.smallGrid = data;
    }
  },
}
</script>

<style>

</style>
