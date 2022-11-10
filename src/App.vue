<script>

import SiteHeader from "./components/SiteHeader.vue"
import SiteContent from "./components/SiteContent.vue"
import SiteReferences from "./components/SiteReferences.vue"

export default {
  name: 'App',
  components: {
    SiteHeader,
    SiteContent,
    SiteReferences
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
  </main>


</template>

<style scoped>

</style>
