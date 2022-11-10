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
        <div class="container">
            <div class="list" v-for="item in links">
                <h5>{{ item.title }}</h5>
                <ul>
                    <li v-for="link in item.list">{{ link }}</li>
                </ul>
            </div>
        </div>
    </section>

</template>



<style>

</style>