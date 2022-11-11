<script>
import links from "../data/links"
import SingleList from "./SingleList.vue"

export default {
    name: "SiteBanner",
    data() {
        return {
            links: links
        }
    },
    components: {
        SingleList
    }
}

</script>



<template>

    <section id="bg_image">
        <div class="container banner">
            <div class="row_banner">

                <div class="col-4">

                    <SingleList v-for="item in links" :title="item.title" :list="item.list" />

                </div>

                <div class="col-6 img_position">
                    <img src="../assets/img/dc-logo-bg.png" alt="">
                </div>
            </div>

        </div>
    </section>

</template>



<style>

</style>