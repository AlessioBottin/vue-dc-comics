<template>
    <div class="single-comic">

        <a href="#">
            <!-- Thumbnail  -->
            <div class="thumbnail">
                <img :src="comicsObject.thumb" :alt="comicsObject.series">
            </div>

            <!-- Comic Name  -->
            <div class="comic-name">
                {{ comicsObject.series }}
            </div>
        </a>

    </div>
</template>

<script>
export default {
    name: 'SingleComic',
    props: ['comicsObject'],
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