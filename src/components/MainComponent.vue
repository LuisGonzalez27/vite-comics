<template>
    <div class="wrapper">
        <div class="my-container">
            <div class="row">
                <ProductComponent v-for="(item, index) in comics" :key="index" :obj="item" />
            </div>
            <div class="d-flex justify-content-center">
                <button class="btn btn-primary text-uppercase strong">loard more</button>
            </div>
        </div>

    </div>
</template>

<script>
import ProductComponent from './ProductComponent.vue';
import { products } from '../data/dc-comics.js';

export default {
    components: {
        ProductComponent
    },
    data() {
        return {
            comics: products,
        }
    }
}
</script>

<style lang="scss" scoped>
@use '../assets/styles/partials/mixins' as *;
@use '../assets/styles/partials/variables' as *;

.wrapper {
    padding: 3rem 0 1.5rem;
}
</style>