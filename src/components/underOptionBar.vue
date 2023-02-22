<script setup lang="ts">
import { library } from "@fortawesome/fontawesome-svg-core";
import {
  faHouse,
  faMoneyBillTransfer,
  faMoneyCheckDollar,
} from "@fortawesome/free-solid-svg-icons";
import { FontAwesomeIcon } from "@fortawesome/vue-fontawesome";

library.add(faHouse);
library.add(faMoneyBillTransfer);
library.add(faMoneyCheckDollar);
</script>

<template>
  <div class="under-wrapper">
    <div class="opt current center">
      <div class="inner-wrap center">
        <div class="icon-wrap">
          <font-awesome-icon icon="fa-solid fa-house" />
        </div>
        <div class="txt-wrap">
          <span class="n-txt arial">Accounts</span>
        </div>
      </div>
    </div>

    <!-- Opt 2 -->
    <div class="opt center">
      <div class="inner-wrap center">
        <div class="icon-wrap">
          <font-awesome-icon icon="fa-solid fa-money-check-dollar" />
        </div>
        <div class="txt-wrap">
          <span class="n-txt arial">Deposit</span>
        </div>
      </div>
    </div>

    <!-- opt 3 -->

    <div class="opt center">
      <div class="inner-wrap center">
        <div class="icon-wrap">
          <font-awesome-icon icon="fa-solid fa-money-bill-transfer" />
        </div>
        <div class="txt-wrap">
          <span class="n-txt arial">transfer</span>
        </div>
      </div>
    </div>
  </div>
</template>

<style lang="sass" scoped>

.center
    display: flex
    justify-content: center
    align-items: center

.under-wrapper
    background: #1F2329
    width: inherit
    height: 80px
    box-shadow: 0px -6px 12px rgba(19, 18, 25, 0.5)
    display: grid
    grid-template-columns: repeat(3, 1fr)

.opt
    background: transparent
    width: 100%
    height: auto
    // padding-bottom: 5px
    font-size: 26px
    color: white

    &.current
        color: red
    &:active
        background: red

    .inner-wrap
        width: 100%
        display: flex
        flex-direction: column
        align-items: center
        justify-content: center

        .n-txt
            font-size: 14px
            color: #DBDBDB
</style>
