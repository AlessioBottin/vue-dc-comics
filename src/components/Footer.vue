<template>
    <footer>
        <div class="container">
            <div class="footer-container">

                <!-- Link list  -->
                <div class="link-list">
                    <ul>
                        
                    </ul>
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
    height: 400px;
    width: 100;
    background-image: url(../assets/img/footer-bg.jpg);
    background-repeat: no-repeat;
    background-size: cover;
    overflow: hidden;

    .container {
        .footer-container {
            position: relative;

            .logo-container {
                position: absolute;
                top: -60px;
                right: 0;
            }
        }
    }
}
</style>