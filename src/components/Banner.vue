<template>
    <section class="banner">
        <div class="container">
            <div class="banner-container">
                <a href="#" class="btn btn-blue">current series</a>
            </div>
        </div>
    </section>
</template>

<script>
export default {
    name: 'Banner',
}
</script>

<style lang="scss" scoped>
@import '../style/variables';
@import '../style/utilities';

.banner {
    
    width: 100%;
    background-image: url(../assets/img/jumbotron.jpg);

    .container {
        .banner-container {
            height: 400px;
            position: relative;

            a {
                font-size: 20px;
                position: absolute;
                left: 0;
                bottom: -20px;
            }
        }
    }
}
</style>