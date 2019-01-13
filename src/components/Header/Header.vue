<template>
    <nav class="navbar navbar-dark bg-primary">

        <app-header-item>

            <img src="../../assets/visa-db-brand-logo.png" slot="nav-brand-logo" width="200" height="50">

        </app-header-item>

        <app-header-item>

        </app-header-item>

    </nav>
</template>

<script>
    import HeaderItem from './HeaderItem.vue';

    export default {
        name: "Header",

        components: {
            appHeaderItem: HeaderItem
        },

        data() {
            return {
                navItems: ['Ask Question', 'Passport Ranking', 'Partner', 'News', 'Contact Us']
            }
        }
    }
</script>

<style scoped>

</style>