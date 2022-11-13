<template>
    <div class="wrapper">
        <div class="my-container">
            <div class="buys">
                <div v-for="(item, index) in list" :key="index" class="buy">
                    <img :src="item.img" alt="social">
                    <a :href="item.url">{{ item.link }}</a>
                </div>
            </div>
        </div>
    </div>
</template>

<script>
export default {
    data() {
        return {
            list: [
                {
                    img: '/public/img/buy-comics-digital-comics.png',
                    link: "digital comics",
                    url: "#",
                },
                {
                    img: '/public/img/buy-comics-merchandise.png',
                    link: "dc mercandise",
                    url: "#",
                },
                {
                    img: '/public/img/buy-comics-subscriptions.png',
                    link: "subscription",
                    url: "#",
                },
                {
                    img: '/public/img/buy-comics-shop-locator.png',
                    link: "comic shop locator",
                    url: "#",
                },
                {
                    img: '/public/img/buy-dc-power-visa.svg',
                    link: "dc power visa",
                    url: "#",
                },
            ]
        };
    },
}
</script>

<style lang="scss" scoped>
@use '../../assets/styles/partials/mixins' as*;
@use '../../assets/styles/partials/variables' as*;

.wrapper {
    background-color: $bluedc;
    color: $white;

    .buys {
        @include dflex;
        height: 150px;

        .buy {
            @include dflex;
            width: calc(100% /5);

            img {
                height: 50px;
            }

            a {
                color: $white;
                text-decoration: none;
                text-transform: uppercase;
                padding-left: 15px;

                &:hover {
                    color: $black;
                }
            }
        }

        .buy:last-child img {
            width: 50px;
        }
    }
}
</style>