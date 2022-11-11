<template>
    <footer>
        <FooterLinks />
    </footer>
</template>

<script>
import FooterLinks from './FooterLinks.vue';

export default {
    components: {
        FooterLinks,
    }
}
</script>

<style lang="scss" scoped>
@use '../assets/styles/partials/variables' as *;
@use '../assets/styles/partials/mixins' as *;
</style>