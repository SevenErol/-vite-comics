<script>
export default {
    name: "SiteFooter",
    data() {
        return {
            images: [
                "footer-facebook.png",
                "footer-periscope.png",
                "footer-pinterest.png",
                "footer-twitter.png",
                "footer-youtube.png"
            ]
        }
    },
    methods: {
        getImageUrl(path) {
            return new URL(path, import.meta.url).href
        }
    }
}

</script>



<template>

    <section id="bg_grey">
        <div class="container">
            <div id="site_footer">

                <button>SIGN UP NOW!</button>

                <div class="social">
                    <span>FOLLOW US</span>
                    <img :src="getImageUrl('../assets/img/' + string)" alt="" v-for="string in images">
                </div>
            </div>
        </div>
    </section>

</template>



<style>

</style>