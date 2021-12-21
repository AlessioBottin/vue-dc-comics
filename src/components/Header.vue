<template>
    <header>       
        <div class="header-container">
            <div class="container">

                <!-- logo  -->
                <div class="logo">
                    <img src="../assets/img/dc-logo.png" alt="Logo dc">
                </div>

                <!-- Menu  -->
                <div class="header-menu">
                    <ul>
                        <li 
                            v-for="(link, index) in links" 
                            :key="index"
                            :class="{ active: link.active }"
                        >
                            <a :href="link.href">{{ link.text }}</a>
                        </li>
                    </ul>
                </div>

            </div>
        </div>
    </header>
</template>

<script>
export default {
    name: "Header",
    data: function() {
        return {
            links: [
                {
                    href: '#',
                    text: 'characters',
                    active: false,
                },
                {
                    href: '#',
                    text: 'comics',
                    active: true,
                },
                {
                    href: '#',
                    text: 'movies',
                    active: false,
                },
                {
                    href: '#',
                    text: 'tv',
                    active: false,
                },
                {
                    href: '#',
                    text: 'games',
                    active: false,
                },
                {
                    href: '#',
                    text: 'collectibles',
                    active: false,
                },
                {
                    href: '#',
                    text: 'videos',
                    active: false,
                },
                {
                    href: '#',
                    text: 'fans',
                    active: false,
                },
                {
                    href: '#',
                    text: 'news',
                    active: false,
                },
                {
                    href: '#',
                    text: 'shop',
                    active: false,
                },
            ],
        }
    },
}
</script>

<style lang="scss" scoped>
@import '../style/variables';

header {
    width: 100%;

    .header-container {
        background-color: white;

        .container {
            display: flex;
            justify-content: space-between;

            .logo {
                max-width: 90px;
                vertical-align: middle;

                img {
                    margin-top: 10px;
                }
            }

            .header-menu {

                li {
                    display: inline-block;
                    line-height: 110px;
                    margin: 0 12px;
                    font-size: 14px;
                    text-transform: uppercase;
                    font-weight: bold;
                    color: #596774;

                    &.active {
                        border-bottom: 5px solid $brand_primary_color;
                        color: $brand_primary_color;
                    }

                    a {
                        line-height: 105px;
                        display: inline-block;
                    }
                }
            }
        }
    }
}
</style>