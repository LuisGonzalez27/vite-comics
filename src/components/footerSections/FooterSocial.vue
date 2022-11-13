<template>
    <div class="wrapper">
        <div class="container">
            <a href="#">sign&hyphen;up now&excl;</a>
            <div class="icons">
                <a class="follow" href="">follow us</a>
                <div v-for="(item, index) in list" :key="index">
                    <img :src="item" alt="social">
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
                '/public/img/footer-facebook.png',
                '/public/img/footer-twitter.png',
                '/public/img/footer-youtube.png',
                '/public/img/footer-pinterest.png',
                '/public/img/footer-periscope.png',
            ]
        };
    },
}
</script>

<style lang="scss" scoped>
@use '../../assets/styles/partials/variables' as *;
@use '../../assets/styles/partials/mixins' as *;

.wrapper {
    background-color: $darkgray;
    color: $white;
}

div.container {
    display: flex;
    height: 100px;
    align-items: center;
    justify-content: space-between;
    text-transform: uppercase;
}

a {
    text-decoration: none;
    color: $white;
    border: 1px solid $bluedc;
    padding: 0.5rem 1rem;

    &:hover:not(.follow) {
        background-color: $bluedc;
    }
}

.follow {
    font-weight: 700;
    margin-left: auto;
    border: none;
    color: $bluedc;

    &:hover {
        color: $white;
    }
}

.icons {
    display: flex;
    justify-content: center;
    align-items: center;

    div {
        padding: 10px;
    }

    img {
        cursor: pointer;

        &:hover {
            transform: scale(1.1);
        }
    }
}
</style>