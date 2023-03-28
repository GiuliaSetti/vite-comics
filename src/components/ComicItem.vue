<script>
    export default {
    name: "ComicItem",
        data() {
            return {
            }
        },
        props: {
            cover: String,
            title: String,
        }
}

</script>

<template>
    <!-- contenitore principale -->
    <div class="comic">
        <img :src="cover" alt="cover">
        <div class="comic_title">{{ title }}</div>
    </div>

</template>

<style lang="scss">

    .comic{
        width: calc(100% / 6 - 20px / 6 * 5);
        color: white;

        img{
            width: 100%;
            aspect-ratio: 1/1;
            object-fit: cover;
            object-position: top;
        }

        .comic_title{
            text-transform: uppercase;
            padding-top: 10px;
        }
    }

</style>