<script>
export default {
    data() {
        return {

        }
    }
}
</script>

<template>
    <footer>
        <!-- footer top -->
        <div class="footer-top">
            <div class="container-footer">
                <div class="background-image"></div>
                <div class="logo"></div>
            </div>
            <div class="container">
                <nav>
                    <div class="list">
                        <h4>Dc comics</h4>
                        <ul>
                            <li><a href="#"> Characters</a></li>
                            <li><a href="#"> Comics</a></li>
                            <li><a href="#"> Movies</a></li>
                            <li><a href="#"> TV</a></li>
                            <li><a href="#"> Games</a></li>
                            <li><a href="#"> Videos</a></li>
                            <li><a href="#"> News</a></li>
                        </ul>

                        <h4>Shop</h4>
                        <ul>
                            <li><a href="#"> Shop DC</a></li>
                            <li><a href="#"> Shop DC Collectibles</a></li>
                        </ul>
                    </div>

                    <div class="list">
                        <h4>Dc </h4>
                        <ul>
                            <li><a href="#"> Terms Of Use</a></li>
                            <li><a href="#"> Privacy policy (New)</a></li>
                            <li><a href="#"> Ad Choices</a></li>
                            <li><a href="#"> Advertising</a></li>
                            <li><a href="#"> Jobs</a></li>
                            <li><a href="#"> Subscriptions</a></li>
                            <li><a href="#"> Talent Workshops</a></li>
                            <li><a href="#"> CPSC Certificates</a></li>
                            <li><a href="#"> Retings</a></li>
                            <li><a href="#"> Shop Help</a></li>
                            <li><a href="#"> Contact Us</a></li>
                        </ul>
                    </div>

                    <div class="list">
                        <h4>Sites</h4>
                        <ul>
                            <li><a href="#"> DC</a></li>
                            <li><a href="#"> MAD Magazine</a></li>
                            <li><a href="#"> DC Kids</a></li>
                            <li><a href="#"> DC Universe</a></li>
                            <li><a href="#"> DC Power Visa</a></li>
                        </ul>
                    </div>
                </nav>
            </div>
        </div>

        <!-- footer boottom -->
        <div class="footer-bottom">
            <div class="container container-foot-bot">
                <div class="sign-up">
                    <a href="#">SIGN-UP NOW!</a>
                </div>

                <div class="follow-us">
                    <a href="#">FOLLOW US </a>
                    <figure>
                        <img src="../assets/img/footer-facebook.png" alt="facebook">
                        <img src="../assets/img/footer-twitter.png" alt="twitter">
                        <img src="../assets/img/footer-youtube.png" alt="youtube">
                        <img src="../assets/img/footer-pinterest.png" alt="pinteret">
                        <img src="../assets/img/footer-periscope.png" alt="periscope">
                    </figure>
                </div>

            </div>
        </div>
    </footer>
</template>

<style lang="scss" scoped>
@use '../assets/scss/vars' as *;

.footer-top {
    height: 540px;
    position: relative;
    padding-top: 110px;
}

.container-footer {
    position: absolute;
    top: 0;
    left: 0;
    width: 100%;
    height: 100%;

    ::before {
        content: "";
        position: absolute;
        top: 0;
        left: 0;
        width: 100%;
        height: 100%;
        background-image: url(../assets/img/footer-bg.jpg);
        background-size: cover;
        z-index: -1;
    }

    ::after {
        content: "";
        position: absolute;
        /* top: 4%; */
        left: 55%;
        width: 650px;
        height: 650px;
        background-image: url(../assets/img/dc-logo-bg.png);
        background-size: cover;
        z-index: -1;
    }
}



nav {
    display: flex;

    .list {
        padding-right: 50px;
        z-index: 1;

        h4 {
            text-transform: uppercase;
            color: $white;
            padding: 10px 0;
        }

        a {
            color: $grey;
            font-weight: 300;
            font-size: 12px;
        }
    }
}



.footer-bottom {
    height: 110px;
    background-color: $darkGrey;
}

.container-foot-bot {
    height: 100%;
    display: flex;
    align-items: center;
    justify-content: space-between;
}

.sign-up a {
    color: $white;
    font-size: 18px;
    font-weight: 500;
    border: 2px solid $blue;
    padding: 10px;
}

.follow-us {
    display: flex;
    align-items: center;

    a {
        color: $blue;
        font-size: 20px;
        font-weight: 700;
        padding-right: 25px;
    }

    img {
        padding-right: 20px;
        cursor: pointer;
    }
}
</style>