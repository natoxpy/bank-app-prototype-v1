<script setup lang="ts">
import BankCards from "@/components/bankAccCards.vue";
</script>

<template>
  <main>
    <div class="top">
      <div class="greet-wrap">
        <span class="top-customer-text arial">Hello, Customer.</span>
      </div>
    </div>
    <BankCards />
  </main>
</template>

<style lang="sass" scoped>
.top
  width: 100%
  height: 100px
.greet-wrap
  display: flex
  align-items: center
  padding-left: 50px
  height: 100px
.top-customer-text
  color: white
  font-size: 26px
</style>
