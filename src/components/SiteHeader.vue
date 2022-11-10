<script>

export default {
    name: "SiteHeader",
    data() {
        return {
            navMenu: [
                {
                    text: "characters",
                    href: "#"
                },
                {
                    text: "comics",
                    href: "#"
                },
                {
                    text: "movies",
                    href: "#"
                },
                {
                    text: "tv",
                    href: "#"
                },
                {
                    text: "games",
                    href: "#"
                },
                {
                    text: "collectibles",
                    href: "#"
                },
                {
                    text: "videos",
                    href: "#"
                },
                {
                    text: "fans",
                    href: "#"
                },
                {
                    text: "news",
                    href: "#"
                },
                {
                    text: "shop",
                    href: "#"
                }
            ]
        }
    }
}

</script>



<template>

    <header id="site-header">
        <div class="logo">
            <img src="../assets/img/dc-logo.png" alt="">
        </div>
        <nav class="navbar">
            <a :href="item.href" v-for="item in navMenu">
                {{ item.text.toUpperCase() }}
            </a>
        </nav>
    </header>

</template>



<style>

</style>