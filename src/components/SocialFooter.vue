<template>
    <footer>
        <div class="container">
            <div class="social-footer-container">

                <!-- Sign up button  -->
                <div class="sign-up">
                    <a href="#" class="btn btn-regular btn-transparent">sign up now!</a>
                </div>

                <!-- Social  -->
                <div class="social">
                    <div class="cta">follow us</div>

                    <div class="social-list">
                        <ul>
                            <li>
                                <img src="../assets/img/footer-facebook.png" alt="fb logo">
                            </li>
                            <li>
                                <img src="../assets/img/footer-twitter.png" alt="twitter logo">
                            </li>
                            <li>
                                <img src="../assets/img/footer-youtube.png" alt="yt logo">
                            </li>
                            <li>
                                <img src="../assets/img/footer-pinterest.png" alt="pinterest logo">
                            </li>
                            <li>
                                <img src="../assets/img/footer-periscope.png" alt="periscope logo">
                            </li>
                        </ul>
                    </div>
                </div>
            </div>
        </div>
    </footer>
</template>

<script>
export default {
    name: 'SocialFooter'
}
</script>

<style lang="scss" scoped>
@import '../style/variables';
@import '../style/utilities';

footer {
    background-color: #303030;

    .container {
        .social-footer-container {
            padding: 30px 0;
            display: flex;
            align-items: center;
            justify-content: space-between;

            .social {
                display: flex;
                align-items: center;

                // Cta 
                .cta {
                    color: $brand_primary_color;
                    font-size: 22px;
                    font-weight: bold;
                    text-transform: uppercase;
                    margin-right: 10px;
                }

                // Logos 
                .social-list {
                    ul {
                        li {
                            display: inline-block;
                            margin-left: 15px;
                        }
                    }
                }
            }
        }
    }
}
</style>