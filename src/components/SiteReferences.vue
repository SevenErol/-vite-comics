<script>
import references from "../data/references"
import SingleReference from "./SingleReference.vue"

export default {
    name: "SiteReferences",
    data() {
        return {
            cols: references
        }
    },

    components: {
        SingleReference
    }
}

</script>



<template>

    <section id="bg_blue">

        <div class="container">
            <div class="row">

                <SingleReference v-for="item in cols" :img="item.img" :text="item.text" />

            </div>
        </div>

    </section>

</template>



<style>

</style>