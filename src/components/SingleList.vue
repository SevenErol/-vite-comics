<script>
export default {
    name: "SingleList",
    props: {
        title: String,
        list: Array
    }
}

</script>

<template>


    <div class="list">
        <h3>{{ title.toUpperCase() }}</h3>
        <ul>
            <li v-for="link in list">{{ link }}</li>
        </ul>
    </div>

</template>