<script>
import cards from "../data/cards.js";
import ComicBook from "./ComicBook.vue"

export default {
    name: "ComicBookList",
    data() {
        return {
            comicList: cards
        }
    },

    components: {
        ComicBook
    }

}
</script>

<template>

    <ComicBook v-for="comic in comicList" :src="comic.thumb" :title="comic.series" />

</template>