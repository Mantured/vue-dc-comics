<template>
    <div class="comic-card">
        <a href="">
            <img :src="comicObj.thumb" :alt="comicObj.series" />
            <h4>{{ comicObj.series }}</h4>
        </a>
    </div>
</template>

<script>
/* import comics from "../assets/dc-comics.json"; */
export default {
    name: "IndexProduct",
    /* data: function () {
    const obj = JSON.parse(comics)
  }, */
    props: ["comicObj"],
};
</script>

<style lang="scss" scoped>
div.comic-card {
    width: calc(100% / 6);
    padding: 0.5rem;
    a {
        text-decoration: none;
        color: white;
        img {
            width: 80%;
            height: 80%;
            margin-bottom: 1rem;
        }
        h4 {
            text-transform: uppercase;
        }
    }
}
</style>
