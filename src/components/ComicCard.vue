<template>
  <div>
    <div class="cards-container">
        <div v-for="comic,index in comics" :key="index" class="card">
            <div class="card-image">
                <img :src="comics[index].thumb" alt="">
            </div>
            <div class="card-text">
                {{ comics[index].series }}
            </div>
        </div>
    </div>
  </div>
</template>

<script>
import ComicData from "../assets/dc-comics.json"
    export default {
        name: "ComicCard",
        components: {
        },
        data () {
            return {
                comics: ComicData
            }
        }

    }
</script>

<style scoped lang="scss">
    // COMICS
    .cards-container{
        width: 97%;
        margin: 0 auto;
        display: flex;
        justify-content: space-between;
        flex-wrap: wrap;
    }
    .card{
        width: calc(86% / 6);
        height: calc(100% / 2);
        margin-bottom: 3rem;
    }
    .card-image{
        width: 100%;
    }
    .card-image img{
        width: 100%;
        object-fit: cover;
        object-position: top;
        aspect-ratio: 1;
    }
    .card-text{
        height: 30%;
        padding: 1rem 0;
    }
</style>