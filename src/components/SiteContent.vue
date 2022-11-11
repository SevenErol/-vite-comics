<script>
import ComicBookList from './ComicBookList.vue';

export default {
    name: "SiteContent",

    components: {
        ComicBookList
    }
}
</script>



<template>

    <section id="bg_black">
        <div class="container">
            <div class="content">
                <div class="row">
                    <ComicBookList />
                </div>
            </div>

            <div class="centered_button">
                <button>LOAD MORE</button>
            </div>

            <div class="disclaimer">
                <p>CURRENT SERIES</p>
            </div>

        </div>

    </section>

</template>

<style lang="scss" scoped>
.container {
    position: relative;
}
</style>


