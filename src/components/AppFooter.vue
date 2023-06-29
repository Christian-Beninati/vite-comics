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

        </div>
    </footer>
</template>

<style scoped>
.footer-top {
    height: 540px;
    position: relative;
    padding: 40px 0;
}

.container-footer {
    position: absolute;
    top: 0;
    left: 0;
    width: 100%;
    height: 100%;
}

.container-footer::before {
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

.container-footer::after {
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

nav {
    display: flex;
}

.list {
    padding-right: 50px;
}

h4 {
    text-transform: uppercase;
    color: white;
    padding: 10px 0;
}


a {
    color: #959595;
    font-weight: 300;
    font-size: 12px;
}

.footer-bottom {
    height: 110px;
    background-color: #303030;
}
</style>