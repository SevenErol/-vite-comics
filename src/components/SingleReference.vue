<script>
export default {
    name: "SingleReference",
    props: {
        img: String,
        text: String
    },
    methods: {
        getImageUrl(path) {
            return new URL(path, import.meta.url).href
        }
    }
}

</script>

<template>

    <div class="col">

        <img :src="getImageUrl('../assets/img/' + img)" :alt="text"
            :class="img === 'buy-comics-shop-locator.png' ? 'locator' : ''">
        <p>{{ text.toUpperCase() }}</p>

    </div>


</template>