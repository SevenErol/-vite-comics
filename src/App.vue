<script>

import SiteHeader from "./components/SiteHeader.vue"
import SiteContent from "./components/SiteContent.vue"

export default {
  name: 'App',
  components: {
    SiteHeader,
    SiteContent
  }
}

</script>

<template>

  <div class="container">
    <SiteHeader />
  </div>

  <main>
    <SiteContent />
  </main>


</template>

<style scoped>

</style>
