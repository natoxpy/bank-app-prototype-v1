<script lang="ts" setup>
const props = defineProps({
  last4Digits: {
    type: String,
    required: true,
  },
  balance: {
    type: Number,
    required: true,
  },
});
</script>

<template>
  <div class="account">
    <div class="top">
      <span class="top-text arial">
        CLEAR ACCESS ACCOUNT BANKING ....{{ props.last4Digits }}
      </span>
    </div>
    <div class="money-mid">
      <span class="money-mid-text arial">
        {{
          new Intl.NumberFormat("us", {
            style: "currency",
            currency: "USD",
          }).format(props.balance)
        }}
      </span>
    </div>
    <div class="under-title">
      <span class="aval-acc arial"> Available Balance </span>
    </div>
  </div>
</template>

<style lang="sass" scoped>

.account
  background: #191919
  width: 100%
  padding: 15px 20px
  border-radius: 5px
  display: grid
  row-gap: 10px
.top-text
  color: white
  font-size: 12px

.money-mid-text
  color: white
  font-size: 26px

.aval-acc
  color: #DBDBDB
  font-size: 12px
</style>
