<template>
  <div class="container">
    <Nuxt />
  </div>
</template>

<script lang="ts">
import Vue from 'vue'
import ToolBar from '../components/ToolBar.vue'
import Login from './login.vue'

export default Vue.extend({
  name: 'Home',
  components: { ToolBar, Login },
  layout: 'home',
})
</script>

<style>
</style>
