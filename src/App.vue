<script>

// imported Vue components
import SiteHeader from "./components/SiteHeader.vue"
import SiteContent from "./components/SiteContent.vue"
import SiteReferences from "./components/SiteReferences.vue"
import SiteBanner from "./components/SiteBanner.vue"
import SiteFooter from "./components/SiteFooter.vue"

export default {
  name: 'App',
  components: {
    SiteHeader,
    SiteContent,
    SiteReferences,
    SiteBanner,
    SiteFooter
  }
}

</script>

<template>

  <!-- site header with container -->
  <div class="container">
    <SiteHeader />
  </div>

  <!-- site main page with sections -->
  <main>

    <!-- section site content -->
    <SiteContent />

    <!-- section site references -->
    <SiteReferences />

    <!-- section site banner -->
    <SiteBanner />

  </main>

  <!-- site footer  -->
  <SiteFooter />


</template>

<style scoped>

</style>
