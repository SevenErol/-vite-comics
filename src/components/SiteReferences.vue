<script>

export default {
    name: "SiteReferences",
    data() {
        return {
            cols: [
                {
                    img: "buy-comics-digital-comics.png",
                    text: "digital comics"
                },
                {
                    img: "buy-comics-merchandise.png",
                    text: "dc merchandise"
                },
                {
                    img: "buy-comics-shop-locator.png",
                    text: "subscriptions"
                },
                {
                    img: "buy-comics-subscriptions.png",
                    text: "comic shop locator"
                },
                {
                    img: "buy-dc-power-visa.svg",
                    text: "dc power visa"
                }
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

    <section id="bg_blue">

        <div class="container">
            <div class="row">
                <div class="col" v-for="item in cols">

                    <img :src="getImageUrl('../assets/img/' + item.img)" alt=""
                        :class="item.img === 'buy-comics-shop-locator.png' ? 'locator' : ''">
                    <p>{{ item.text.toUpperCase() }}</p>

                </div>
            </div>
        </div>

    </section>

</template>



<style>

</style>