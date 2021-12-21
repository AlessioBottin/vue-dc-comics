<template>
<!-- Mi sono dimenticato di mettere il tag a su tutte le li  -->
    <footer>
        <div class="container">
            <div class="footer-container">

                <!-- Link Container -->
                <div class="link-container">
                    
                    <!-- Left  -->
                    <div class="col col-l">

                        <!-- Comics  -->
                        <div class="comics">

                            <!-- Title  -->
                            <h3>dc shop</h3>

                            <!-- Link list  -->
                            <ul>
                                <li>Character</li>
                                <li>Comics</li>
                                <li>Movies</li>
                                <li>TV</li>
                                <li>Games</li>
                                <li>Videos</li>
                                <li>News</li>
                            </ul>
                        </div>

                        <!-- Shop  -->
                        <div class="shop">

                            <!-- Title  -->
                            <h3>shop</h3>

                            <!-- Link List  -->
                            <ul>
                                <li>DC Shop</li>
                                <li>DC Collectibles</li>
                            </ul>

                        </div>

                    </div>

                    <!-- Center  -->
                    <div class="col col-center">

                        <!-- Dc  -->
                        <div class="comics">

                            <!-- Title  -->
                            <h3>dc</h3>

                            <!-- Link list  -->
                            <ul>
                                <li>Terms of use</li>
                                <li>Priacy Policy</li>
                                <li>Ad choices</li>
                                <li>Advertising</li>
                                <li>Jobs</li>
                                <li>Subscriptions</li>
                                <li>Talent workshop</li>
                                <li>CPSC Certificates</li>
                                <li>Ratings</li>
                                <li>Shop help</li>
                                <li>Contact us</li>
                            </ul>

                        </div>

                    </div>

                    <!-- Right  -->
                    <div class="col col-r">

                        <!-- Sites  -->
                        <div class="sites">

                            <!-- Title  -->
                            <h3>Sites</h3>

                            <!-- Link list  -->
                            <ul>
                                <li>DC</li>
                                <li>MAD Magazine</li>
                                <li>DC Kids</li>
                                <li>DC Universe</li>
                                <li>DC Power Visa</li>
                            </ul>

                        </div>

                    </div>

                </div>

                <!-- Image  -->
                <div class="logo-container">
                    <img src="../assets/img/dc-logo-bg.png" alt="dc logo">
                </div>

            </div>
        </div>
    </footer>
</template>

<script>
export default {
    name: "Footer",
}
</script>

<style lang="scss" scoped>
@import '../style/variables';

footer {
    width: 100%;
    background-image: url(../assets/img/footer-bg.jpg);
    background-repeat: no-repeat;
    background-size: cover;
    overflow: hidden;

    .container {
        .footer-container {
            position: relative;
            padding: 50px 0;

            // Link container 
            .link-container {
                display: flex;

                .col {
                    margin-right: 40px;

                    div {
                        margin-bottom: 20px;

                        // Title 
                        h3 {
                            margin-bottom: 20px;
                            color: white;
                            text-transform: uppercase;
                            font-size: 18px;
                        }

                        // Link 
                        ul {
                            li {
                                font-size: 13px;
                                color: rgb(156, 156, 156);
                                margin-bottom: 5px;
                            }
                        }
                    }
                }
                
            }

            // Logo 
            .logo-container {
                position: absolute;
                top: -60px;
                right: 0;
            }
        }
    }
}
</style>