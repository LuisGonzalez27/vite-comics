<template>
    <div class="col">
        <div class="img-comic">
            <img :src="obj.thumb" :alt="obj.series">
        </div>
        <h4>{{ obj.series }}</h4>
    </div>
</template>

<script>
export default {
    name: 'ProductComponent',
    props: [
        'obj'
    ]
}
</script>

<style lang="scss" scoped>
@use '../assets/styles/partials/variables' as *;
@use '../assets/styles/partials/mixins' as *;

.col {
    flex-basis: calc(100% / 6);
}

.img-comic {
    height: 170px;
    overflow: hidden;
}

h4 {
    color: $white;
    font-size: 12px;
    text-transform: uppercase;
    padding: 1rem 0;
}
</style>