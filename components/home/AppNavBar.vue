<template>
  <nav class="navbar navbar-main navbar-expand-lg navbar-light border-bottom custom-top-nav" >
    <div class="container">

      <button class="navbar-toggler" type="button" data-toggle="collapse" data-target="#main_nav" aria-controls="main_nav" aria-expanded="false" aria-label="Toggle navigation">
        <span class="navbar-toggler-icon"></span>
      </button>

      <div class="collapse navbar-collapse" id="main_nav">
        <ul class="navbar-nav mx-auto list-inline">
          <li class="nav-item">
            <a class="nav-link" href="#">
              <BuyLogo :height="25" :width="25" />
              &nbsp; <span class="h5" style="color: #3858a5" >Buy</span>
            </a>
          </li>

          <li class="nav-item">
            <a class="nav-link" href="#">
              <SwapLogo :height="20" :width="20" />
              &nbsp; <span class="h5" style="background: -webkit-linear-gradient(right, #E87C28, #3858a5); -webkit-background-clip: text; -webkit-text-fill-color: transparent;">Swap</span>
            </a>
          </li>

          <li class="nav-item">
            <a class="nav-link" href="#">
              <SellLogo :height="25" :width="25"/>
              &nbsp; <span class="h5" style="color: #E87C28">Sell</span>
            </a>
          </li>
          <li class="nav-item dropdown">
            <a class="nav-link dropdown-toggle caret-off" data-toggle="dropdown" href="#">
              <MoreLogo :height="25" :width="25"/>
              <span class="h5" style="color: #3858a5">More</span>
            </a>
            <div class="dropdown-menu">
              <a class="dropdown-item" href="#">Foods and Drink</a>
              <a class="dropdown-item" href="#">Home interior</a>
              <div class="dropdown-divider"></div>
              <a class="dropdown-item" href="#">Category 1</a>
              <a class="dropdown-item" href="#">Category 2</a>
              <a class="dropdown-item" href="#">Category 3</a>
            </div>
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

</style>
