<template lang="jade">
    #app
        main-header
        main.main
            .container.flex
                side-nav
                router-view.flex__item
        main-footer
</template>

<script>
    import MainHeader from './header.vue';
    import MainFooter from './footer.vue';
    import SideNav from './side-nav.vue';

    export default {
        components: {
            MainHeader,
            MainFooter,
            SideNav
        },
        data() {
            return {
                loading: false
            };
        },
        createdfvg() {
            this.init();
        },
        methods: {
            load() {
            },
            init() {
                // const that = this;
                // this.load().then(res => {});
            }
        }
    };
</script>

<style lang="scss">
    @import "../stylesheets/app.scss";
</style>
