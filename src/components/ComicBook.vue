<script>


export default {
    name: "ComicBook",
    props: {
        src: String,
        title: String
    }
}
</script>




<template>
    <div class="col-2">
        <img :src="src" :alt="title">
        <h6>{{ title }}</h6>
    </div>

</template>

