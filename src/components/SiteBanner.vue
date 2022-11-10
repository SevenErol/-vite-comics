<script>
export default {
    name: "SiteBanner",
    data() {
        return {
            links: [
                {
                    title: "dc comics",
                    list: [
                        "characters",
                        "comics",
                        "movies",
                        "tv",
                        "games",
                        "videos",
                        "news"
                    ]
                },
                {
                    title: "shop",
                    list: [
                        "shop dc",
                        "shop dc collectibles"
                    ]
                },
                {
                    title: "dc",
                    list: [
                        "terms of use",
                        "Privacy policy(new)",
                        "Ad choices",
                        "Advertising",
                        "Jobs",
                        "Subscriptions",
                        "Talent Workshops",
                        "CPSC certificate",
                        "Ratings",
                        "Shop help",
                        "Contact Us"
                    ]
                },
                {
                    title: "Sites",
                    list: [
                        "DC",
                        "MAD Magazine",
                        "DC Kids",
                        "DC Universe",
                        "DC Power Visa"
                    ]
                }
            ]
        }
    }
}

</script>



<template>

    <section id="bg_image">
        <div class="container banner">
            <div class="row_banner">
                <div class="col-4">
                    <div class="list" v-for="item in links">
                        <h3>{{ item.title.toUpperCase() }}</h3>
                        <ul>
                            <li v-for="link in item.list">{{ link }}</li>
                        </ul>
                    </div>
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