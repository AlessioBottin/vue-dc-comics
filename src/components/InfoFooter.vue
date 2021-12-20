<template>
    <div class="info-footer">
        <div class="container">
            <div class="content-container">
                <div 
                    class="item-box"
                    v-for="(item, index) in items"
                    :key="index"
                >   
                    <!-- Img  -->
                    <img 
                        :src="require('../assets/img/buy-' + item.imgSrc)" 
                        :alt="item.text"
                    >
                    <!-- Text  -->
                    <div>{{ item.text }}</div>
                </div>
            </div>
        </div>
    </div>  
</template>

<script>
export default {
    name: "InfoFooter",
    data: function() {
        return {
            items: [
                {
                    imgSrc: 'comics-digital-comics.png',
                    text: 'digital comics'
                },
                {
                    imgSrc: 'comics-merchandise.png',
                    text: 'dc merchandise'
                },
                {
                    imgSrc: 'comics-subscriptions.png',
                    text: 'subscription'
                },
                {
                    imgSrc: 'comics-shop-locator.png',
                    text: 'comic shop locator'
                },
                {
                    imgSrc: 'dc-power-visa.svg',
                    text: 'dc power visa'
                },
            ],
        }
    }
}
</script>

<style lang="scss" scoped>
@import '../style/variables';

.info-footer {
    background-color: $brand_primary_color;
    color: white;
    padding: 50px 0px;
    text-transform: uppercase;
    font-size: 15px;

    .container {
        .content-container {
            display: flex;
            justify-content: space-between;
            padding: 0 30px;

            .item-box {
                display: flex;
                align-items: center;

                img {
                    max-width: 45px;
                    width: 45px;
                    margin-right: 10px;
                }
            }
        }
    }
}
</style>