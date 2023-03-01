<script setup lang="ts">
import { RouterLink, RouterView } from 'vue-router'
import { Icon } from '@vicons/utils'
import { NButton, NDivider, NAvatar } from 'naive-ui'
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
    <n-space> <n-avatar src="@sicons/fluent/User.svg" size="small" /> <n-divider /> </n-space>
  </header>
  <body>
    <n-button @click="addCounter(1)">Click To Add!</n-button>
    <p>{{ counter.count }}</p>
  </body>
</template>

<style scoped></style>
