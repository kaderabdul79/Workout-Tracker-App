<template>
  <div>
    <SiteNavigation />
    <router-view />
  </div>
</template>

<script>
import SiteNavigation from './components/SiteNavigation.vue'
export default {
  components: { SiteNavigation },

}
</script>

<style>

</style>