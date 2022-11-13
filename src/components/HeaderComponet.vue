<template>
    <header class="my-container">
        <a href="#">
            <img src="../assets/img/dc-logo.png" alt="DC Logo">
        </a>
        <nav>
            <ul>
                <li v-for="(link, index) in links" :key="index">
                    <a :href="link.url" :class="{ 'active': link.current }">
                        {{ link.text }}
                    </a>
                </li>
            </ul>
        </nav>
    </header>
</template>

<script>
export default {
    name: 'HeaderComponent',
    data() {
        return {
            links: [
                {
                    text: "Characters",
                    url: "#",
                    current: false,
                },
                {
                    text: "Comics",
                    url: "#",
                    current: true,
                },
                {
                    text: "Movies",
                    url: "#",
                    current: false,
                },
                {
                    text: "Tv",
                    url: "#",
                    current: false,
                },
                {
                    text: "Games",
                    url: "#",
                    current: false,
                },
                {
                    text: "Collectibles",
                    url: "#",
                    current: false,
                },
                {
                    text: "Videos",
                    url: "#",
                    current: false,
                },
                {
                    text: "Fans",
                    url: "#",
                    current: false,
                },
                {
                    text: "News",
                    url: "#",
                    current: false,
                },
                {
                    text: "Shop",
                    url: "#",
                    current: false,
                },
            ]
        }
    }
}
</script>

<style lang="scss" scoped>
@use '../assets/styles/partials/mixins' as*;
@use '../assets/styles/partials/variables' as*;

header {
    text-align: center;
    display: flex;
    justify-content: space-between;
    align-items: center;

    nav {
        height: 120px;
    }

    ul {
        list-style: none;
        height: 120px;
        @include dflex;

        li a {
            display: inline-block;
            padding: 0 1rem;
            text-decoration: none;
            font-weight: 600;
            color: $graytext;
            text-transform: uppercase;
            line-height: 110px;

            &.active,
            &:hover {
                color: $bluedc;
                border-bottom: 5px solid $bluedc;
                border-top: 5px solid $white;
            }
        }
    }
}
</style>