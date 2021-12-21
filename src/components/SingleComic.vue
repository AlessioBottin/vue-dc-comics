<template>
    <div class="single-comic">

        <a href="#">
            <!-- Thumbnail  -->
            <div class="thumbnail">
                <img src="https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2018/09/AC1000_DLX_162-001_HD_5ba13723281ab0.37845353.jpg?itok=ZsI-C5eX" alt="">
            </div>

            <!-- Comic Name  -->
            <div class="comic-name">
                action comics
            </div>
        </a>

    </div>
</template>

<script>
export default {
    name: 'SingleComic',
}
</script>

<style lang="scss" scoped>
@import '../style/variables';
@import '../style/utilities';

.single-comic {
    margin: 0 20px 20px;
    width: calc( (100% / 6) - 40px);

    // Thumb 
    .thumbnail {
        margin-bottom: 20px;      
        height: 175px;
        overflow-y: hidden;   
    }

    // Comic Name 
    .comic-name {
        text-transform: uppercase;
        color: white;
        font-size: 15px;
    }
}
</style>