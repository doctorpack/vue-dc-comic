<template>
  <div>
    <section>
        <div class="upper-main-adjustments">
            <div class="upper-main-jumbotron">

            </div>
            <div class="container">
                <div class="comics-container">
                    <div class="label">
                        <span>CURRENT SERIES</span>
                    </div>
                    <ComicCard />
                </div>
            </div>
            <div class="container">
                <div class="button-adjustments">
                    <span>LOAD MORE</span>
                </div>
            </div>
        </div>
    </section>
    <section>
        <MyCards/>
    </section>
  </div>
</template>

<script>
    import MyCards from "./MyCard.vue"
    import ComicCard from "./ComicCard.vue"
    export default {
        name: "MyMain",
        components:{
            MyCards,
            ComicCard
        }
}
</script>

<style scoped lang="scss">
    @import "../style/variables.scss";
    @import '../style/common.scss';
    .upper-main-adjustments{
        background-color: black;
        color: white;
    }
    .upper-main-jumbotron{
        background-image: url(../assets/img/jumbotron.jpg);
        height: 400px;
    }
    .comics-container{
        padding-top: 3rem;
        position: relative;
    }
    // COMICS CARDS SECTION
    .label{
        display: inline-block;
        padding: 0.7rem 1.3rem;
        background-color: $brand_main_color;
        position: absolute;
        top: -30px;
        left: 0;
    }
    .label span{
        font-size: 1.6rem;
        font-weight: bold;
    }
    .button-adjustments{
        display: flex;
        justify-content: center;
        padding: 1.5rem 0;
    }
    .button-adjustments span{
        padding: 0.5rem 3rem;
        background-color: $brand_main_color;
        font-weight: bold;
    }
</style>