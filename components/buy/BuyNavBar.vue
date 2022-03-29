<template>
  <nav class="navbar navbar-main navbar-expand-lg navbar-light border-bottom custom-top-nav" >
    <div class="container">

      <button class="navbar-toggler" type="button" data-toggle="collapse" data-target="#main_nav" aria-controls="main_nav" aria-expanded="false" aria-label="Toggle navigation">
        <span class="navbar-toggler-icon"></span>
      </button>

      <div class="collapse navbar-collapse" id="main_nav">
        <ul class="navbar-nav mx-auto list-inline menu-category buy-header-nav">
          <li class="nav-item m-1">
            <a class="nav-link d-inline caret-off" href="#">
              <img width="22" src="~/assets/images/logo/phone.png">
              <span class="h6" style="color: #3858a5" >Sell SmartPhone</span>
            </a>
          </li>
          <li class="nav-item m-1">
            <a class="nav-link d-inline caret-off" href="#">
              <img width="25" src="~/assets/images/logo/laptop.png">
              <span class="h6" style="color: #3858a5" >Sell Laptop</span>
            </a>
          </li>
          <li class="nav-item m-1">
            <a class="nav-link d-inline caret-off" href="#">
              <img width="25" src="~/assets/images/logo/motorcycle.png">
              <span class="h6" style="color: #3858a5" >Sell Bike</span>
            </a>
          </li>
          <li class="nav-item m-1">
            <a class="nav-link d-inline caret-off" href="#">
              <img width="25" src="~/assets/images/logo/vehicles.png">
              <span class="h6" style="color: #3858a5" >Sell Car</span>
            </a>
          </li>

          <li class="nav-item m-1 has-submenu">
            <a class="nav-link caret-off d-inline" href="#">
              <MoreLogo :height="20" :width="20"/>
              &nbsp; <span class="h6" style="color: #1779b5">More</span>
            </a>
            <ul class="submenu" >
              <li><a href="#">Submenu name</a></li>
              <li><a href="#">Great submenu</a></li>
              <li><a href="#">Another menu</a></li>
              <li><a href="#">Some others</a></li>
            </ul>
          </li>
        </ul>
      </div> <!-- collapse .// -->
    </div> <!-- container .// -->
  </nav>
</template>

<script>
import SellLogo from '~/components/custom/SellLogo.vue'
import SwapLogo from '~/components/custom/SwapLogo.vue'
import BuyLogo from '~/components/custom/BuyLogo.vue'
import MoreLogo from '../custom/MoreLogo.vue'
export default {
  components: { SwapLogo, SellLogo, BuyLogo, MoreLogo },

}
</script>

<style>
  /* remove bottom border  */
  .buy-header-nav li {
    border-bottom: unset
  }

  /* show header submenu on bottom */
  .buy-header-nav ul {
    left: unset !important;
    top: 120% !important;
  }

  /* change color ob header submenu hover */
  .buy-header-nav > .has-submenu > .submenu a:hover{
    background: #eda224 !important;
  }

  .buy-header-nav > .nav-item  a:hover   span{
    color: #eda224 !important;
    transition: all 0.20s ease-out;
  }
</style>
