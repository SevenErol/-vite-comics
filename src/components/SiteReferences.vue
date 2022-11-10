<script>

export default {
    name: "SiteReferences",
    data() {
        return {
            cols: [
                {
                    imgURL: "buy-comics-digital-comics.png",
                    text: "digital comics"
                },
                {
                    imgURL: "buy-comics-merchandise.png",
                    text: "dc merchandise"
                },
                {
                    imgURL: "buy-comics-shop-locator.png",
                    text: "subscriptions"
                },
                {
                    imgURL: "buy-comics-subscriptions.png",
                    text: "comic shop locator"
                },
                {
                    imgURL: "buy-dc-power-visa.svg",
                    text: "dc power visa"
                }
            ]
        }
    }
}

</script>



<template>

    <div class="container">
        <div class="row">
            <div class="col" v-for="item in cols">
                <img :src="'../assets/img/' + item.imgURL" alt="">
                <p>{{ item.text }}</p>
            </div>
        </div>
    </div>

</template>



<style>

</style>