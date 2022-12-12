<template>
  <div>
    <div class="footer-adjustments">
        <div class="container">
            <div class="footer-alignments">
                <nav class="footer-nav">
                    <div class="footer-box">
                        <h4>DC COMICS</h4>
                        <ul>
                            <li><a href="">Characters</a></li>
                            <li><a href="">Comics</a></li>
                            <li><a href="">Movies</a></li>
                            <li><a href="">TV</a></li>
                            <li><a href="">Games</a></li>
                            <li><a href="">Videos</a></li>
                            <li><a href="">News</a></li>
                        </ul>
                        <h4>SHOP</h4>
                        <ul>
                            <li><a href="">Shop DC</a></li>
                            <li><a href="">Shop DC Collectibles</a></li>
                        </ul>
                    </div>
                    <div class="footer-box">
                        <h4>DC</h4>
                        <ul>
                            <li><a href="">Terms of Use</a></li>
                            <li><a href="">Privacy Policy</a></li>
                            <li><a href="">Ad Choiches</a></li>
                            <li><a href="">Advertising</a></li>
                            <li><a href="">Jobs</a></li>
                            <li><a href="">Subscriptions</a></li>
                            <li><a href="">Talent Workshops</a></li>
                            <li><a href="">CPSC Certificates</a></li>
                            <li><a href="">Ratings</a></li>
                            <li><a href="">Shop Help</a></li>
                            <li><a href="">Contact Us</a></li>
                        </ul>
                    </div>
                    <div class="footer-box">
                        <h4>SITES</h4>
                        <ul>
                            <li><a href="">DC</a></li>
                            <li><a href="">MAD Magazine</a></li>
                            <li><a href="">DC Kids</a></li>
                            <li><a href="">DC Universe</a></li>
                            <li><a href="">DC Power Visa</a></li>
                        </ul>
                    </div>
                </nav>
                <div class="dc-image">
                </div>
            </div>
        </div>
    </div>
    <div class="lower-footer-adjustments">
        <div class="container">
            <div class="lower-footer-alignments">
                <div class="lower-footer-button">
                    <button class="big-button">SIGN UP NOW!</button>
                </div>
                <div class="socials">
                    <div class="lower-footer-text">
                        <span>FOLLOW US</span>
                    </div>
                    <div class="lower-footer-socials">
                        <a href="#"><img src="../assets/img/footer-twitter.png" alt=""></a>                    
                        <a href="#"><img src="../assets/img/footer-facebook.png" alt=""></a>                    
                        <a href="#"><img src="../assets/img/footer-youtube.png" alt=""></a>                   
                        <a href="#"><img src="../assets/img/footer-pinterest.png" alt=""></a>
                        <a href="#"><img src="../assets/img/footer-periscope.png" alt=""></a>
                    </div>
                </div>
            </div>
        </div>
    </div>
  </div>
</template>

<script>
export default {
    name: "MyFooter",
}
</script>

<style>
    @import "../style/variables.scss";
    @import "../style/common.scss";
    /* FOOTER */
    .footer-adjustments{
        background-image: url(../assets/img/footer-bg.jpg);
        background-repeat: no-repeat;
        background-size: cover;
    }
    .footer-alignments{
        display: flex;
        justify-content: space-between;
    }
    .footer-nav{
        display: flex;
    }
    .footer-box{
        height: 380px;
        padding-right: 1rem;
        padding-top: 2rem;
        color: white;
    }
    .dc-image{
        width: 50%;
        background-image: url("../assets/img/dc-logo-bg.png");
        background-repeat: no-repeat;
        background-position-y: center;
    }
    .footer-nav h4{
        font-size: 1.2rem;
    }
    .footer-nav ul{
        margin-top: 0.5rem;
    }
    .footer-nav ul li{
        margin-bottom: 0.5rem;
        font-size: 0.8rem;
    }
    .footer-nav ul li a{
        text-decoration: none;
        color: #959595;
    }
    /* LOWER FOOTER */
    .lower-footer-adjustments{
        background-color: #303030;
    }
    .lower-footer-alignments{
        display: flex;
        justify-content: space-between;
        align-items: center;
    }
    .big-button{
        margin: 2rem 0;
        border: 2px solid #0282f9;
        background-color: #303030;
        color: white;
        padding: 15px 15px;
        font-size: 1.1rem;
        font-weight: bold;
    }
    .lower-footer-text{
        font-size: 1.1rem;
        font-weight: bold;
        color: #0282f9;
    }
    .socials{
        display: flex;
        align-items: center;
    }
    .lower-footer-socials{
        width: 300px;
        margin-left: 1rem;
    }
    .lower-footer-socials img{
        margin: 0 0.4rem;
    }
</style>