<script setup lang="ts">
import { RouterLink, RouterView } from 'vue-router'
import { Icon } from '@vicons/utils'
import { NButton, NLayout, NLayoutContent, NLayoutHeader, NMenu } from 'naive-ui'
import { reactive } from 'vue'
import NavigationBar from './components/NavigationBar.vue'
</script>

<template>
  <main>
    <NavigationBar />
  </main>
</template>

<style scoped></style>
