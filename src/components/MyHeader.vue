<template>
  <div class="container">
    <div class="header-adjustments">
        <div class="logo">
            <img src="../assets/img/dc-logo.png" alt="dc logo">
        </div>
        <nav class="nav">
            <ul>
                <li><a href="">CHARACTERS</a></li>
                <li><a href="">COMICS</a></li>
                <li><a href="">MOVIES</a></li>
                <li><a href="">TV</a></li>
                <li><a href="">GAMES</a></li>
                <li><a href="">COLLECTIBLES</a></li>
                <li><a href="">VIDEOS</a></li>
                <li><a href="">FANS</a></li>
                <li><a href="">NEWS</a></li>
                <li><a href="">SHOP</a></li>
            </ul>
        </nav>
    </div>
  </div>
</template>

<script>

export default {
    name: "MyHeader",
}
</script>

<style scoped lang="scss">
    @import "../style/variables.scss";
    @import '../style/common.scss';
    .header-adjustments{
        height: 120px;
        padding: 1rem 0;
        display: flex;
        justify-content: space-between;
        align-items: center;
    }
    .logo{
        height: 90px;
    }
    .nav{
        width: 60%;
    }
    .nav ul{
        display: flex;
        align-items: center;
        justify-content: space-between;
        border-bottom: 3px solid transparent;
        height: 100%;
    }
    .active{
        border-bottom: 3px solid $brand_main_color;
        color: $brand_main_color;
    }
    li{
        font-size: 0.8rem;
        font-weight: bold;
        height: 100%;
    }
    a{
        color: black;
    }
</style>