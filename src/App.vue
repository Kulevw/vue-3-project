<template>
  <component :is="getLayout">
    <div id="nav">
      <router-link to="/">Home</router-link> |
      <router-link to="/about">About</router-link>
    </div>
    <router-view />
  </component>
</template>

<script>
import TheMainLayout from '@/layouts/TheMainLayout'

export default {
  components: {
    TheMainLayout,
  },
  computed: {
    getLayout() {
      return 'TheMainLayout'
    },
  },
}
</script>

<style>
@import './styles/bootstrap-grid.css';
</style>
