<template>
    <footer>
        <FooterLinks />
        <FooterSocial />
    </footer>
</template>

<script>
import FooterLinks from './footerSections/FooterLinks.vue';
import FooterSocial from './footerSections/FooterSocial.vue';

export default {
    components: {
        FooterLinks,
        FooterSocial
    }
}
</script>

<style lang="scss" scoped>
@use '../assets/styles/partials/variables' as *;
@use '../assets/styles/partials/mixins' as *;
</style>