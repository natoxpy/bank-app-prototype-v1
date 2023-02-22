<script setup lang="ts">
import BankCard from "@/components/bankAccCard.vue";

const defaultCards = [
  {
    l4d: "4343",
    balance: 39043.34,
  },
  {
    l4d: "6343",
    balance: 44.65,
  },
];
</script>

<template>
  <div class="acc-wrapper">
    <!-- vue for loop -->
    <BankCard
      v-for="card in defaultCards"
      :key="card.l4d"
      :last4-digits="card.l4d"
      :balance="card.balance"
    ></BankCard>
  </div>
</template>

<style lang="sass" scoped>
.acc-wrapper
  // background: red
  display: grid
  row-gap: 10px
  width: 100%
  height: auto
  padding: 0 30px
</style>
