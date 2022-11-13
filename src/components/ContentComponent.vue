<template>
    <section class="my-container" id="content">
        <h1>&hyphen;&hyphen;&gt;Content goes here&lt;&hyphen;&hyphen;</h1>
    </section>
</template>

<script>
export default {
    name: 'ContentComponent'
}
</script>

<style lang="scss" scoped>
@use '../assets/styles/partials/mixins' as*;
@use '../assets/styles/partials/variables' as*;

#content {
    display: flex;
    align-items: center;
    height: 150px;
    color: $white;
}
</style>