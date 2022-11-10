<script>

import SiteHeader from "./components/SiteHeader.vue"
import SiteContent from "./components/SiteContent.vue"
import SiteReferences from "./components/SiteReferences.vue"
import SiteBanner from "./components/SiteBanner.vue"
// import SiteFooter from "./components/SiteFooter.vue"

export default {
  name: 'App',
  components: {
    SiteHeader,
    SiteContent,
    SiteReferences,
    SiteBanner,
    // SiteFooter
  }
}

</script>

<template>

  <div class="container">
    <SiteHeader />
  </div>

  <main>
    <SiteContent />

    <SiteReferences />

    <SiteBanner />
  </main>


</template>

<style scoped>

</style>
