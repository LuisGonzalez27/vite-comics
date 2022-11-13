<template>
    <div class="wrapper">
        <div class="container">
            <ul>
                <ul>
                    <li v-for="(item, index) in dcComics" :key="index">
                        <a :href="item.url">{{ item.link }}</a>
                    </li>
                </ul>

                <ul>
                    <li v-for="(item, index) in shop" :key="index">
                        <a :href="item.url">{{ item.link }}</a>
                    </li>
                </ul>
            </ul>
            <ul>
                <li v-for="(item, index) in dc" :key="index">
                    <a :href="item.url">{{ item.link }}</a>
                </li>
            </ul>
            <ul>
                <li v-for="(item, index) in sites" :key="index">
                    <a :href="item.url">{{ item.link }}</a>
                </li>
            </ul>
            <div>
                <img src="../../assets/img/dc-logo-bg.png" alt="">
            </div>
        </div>
    </div>
</template>

<script>
export default {
    data() {
        return {
            dcComics: [
                {
                    link: "Dc Comics",
                    url: "#",
                },
                {
                    link: "Characters",
                    url: "#",
                },
                {
                    link: "Comics",
                    url: "#",
                },
                {
                    link: "Movies",
                    url: "#",
                },
                {
                    link: "TV",
                    url: "#",
                },
                {
                    link: "Games",
                    url: "#",
                },
                {
                    link: "Videos",
                    url: "#",
                },
                {
                    link: "News",
                    url: "#",
                },
            ],
            shop: [
                {
                    link: "Shop",
                    url: "#",
                },
                {
                    link: "Shop DC",
                    url: "#",
                },
                {
                    link: "Shop DC Collectibles",
                    url: "#",
                },
            ],
            dc: [
                {
                    link: "Dc",
                    url: "#",
                },
                {
                    link: "Terms Of Use",
                    url: "#",
                },
                {
                    link: "Privacy Policy(New)",
                    url: "#",
                },
                {
                    link: "Ad Choices",
                    url: "#",
                },
                {
                    link: "Advertising",
                    url: "#",
                },
                {
                    link: "Jobs",
                    url: "#",
                },
                {
                    link: "Subscriptions",
                    url: "#",
                },
                {
                    link: "Talent Workshops",
                    url: "#",
                },
                {
                    link: "CPSC Certificates",
                    url: "#",
                },
                {
                    link: "Ratings",
                    url: "#",
                },
                {
                    link: "Shop Help",
                    url: "#",
                },
                {
                    link: "Contact Us",
                    url: "#",
                },
            ],
            sites: [
                {
                    link: "Sities",
                    url: "#",
                },
                {
                    link: "DC",
                    url: "#",
                },
                {
                    link: "MAD Magazine",
                    url: "#",
                },
                {
                    link: "DC Kids",
                    url: "#",
                },
                {
                    link: "DC Universe",
                    url: "#",
                },
                {
                    link: "DC Power Visa",
                    url: "#",
                },
            ],
        };
    },
}
</script>

<style lang="scss" scoped>
@use '../../assets/styles/partials/mixins' as*;
@use '../../assets/styles/partials/variables' as*;

.wrapper {
    background-image: url("../../assets/img/footer-bg.jpg");
    background-size: cover;
    background-repeat: no-repeat;
    position: relative;
    overflow: hidden;
}

div.container {
    display: flex;

    ul {
        list-style: none;
        padding: 0 1rem 1rem 0;

        li a {
            text-decoration: none;
            color: $graytext;
            padding: 2px 0;
            display: inline-block;

            &:hover {
                color: $bluedc;
            }
        }

        li:first-child a {
            color: $white;
            font-size: 1.5rem;
            padding: 1.5rem 0rem 1rem;
            text-transform: uppercase;
        }
    }
}

img {
    position: absolute;
    right: 10%;
    top: 50%;
    transform: translateY(-50%);
}
</style>