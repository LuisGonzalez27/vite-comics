<template>
    <footer>
        <FooterTop />
        <FooterLinks />
        <FooterSocial />
    </footer>
</template>

<script>
import FooterLinks from './footerSections/FooterLinks.vue';
import FooterSocial from './footerSections/FooterSocial.vue';
import FooterTop from './footerSections/FooterTop.vue';


export default {
    components: {
        FooterLinks,
        FooterSocial,
        FooterTop
    }
}
</script>

<style lang="scss" scoped>
@use '../assets/styles/partials/variables' as *;
@use '../assets/styles/partials/mixins' as *;
</style>