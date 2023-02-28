<script setup lang="ts">
import { RouterLink, RouterView } from 'vue-router'
import { Icon } from '@vicons/utils'
import { NButton } from 'naive-ui'
import { reactive } from 'vue'

const counter = reactive({
  count: 0
})
console.log(counter.count)
function addCounter(amount: any) {
  counter.count += amount
}
</script>

<template>
  <header>
    <img alt="Vue logo" class="logo" src="@/assets/logo.svg" width="125" height="125" />
  </header>
  <body>
    <n-button @click="addCounter">Click To Add!</n-button>
    <p>{{ counter.count }}</p>
  </body>
</template>

<style scoped></style>
