<template>
    <div class="jumbotron">
        <div class="my-container">
            <div class="headline">
                current series
            </div>
        </div>
    </div>
</template>

<script>
export default {

}
</script>

<style lang="scss" scoped>
@use '../assets/styles/partials/mixins' as*;
@use '../assets/styles/partials/variables' as*;

.jumbotron {
    background-image: url('../assets/img/jumbotron.jpg');
    height: 400px;
    background-size: cover;
    position: relative;

    .headline {
        position: absolute;
        bottom: 0px;
        transform: translateY(50%);
        padding: 0.5rem 1rem;
        background-color: $bluedc;
        color: $white;
        text-transform: uppercase;
        font-weight: bold;
    }
}
</style>