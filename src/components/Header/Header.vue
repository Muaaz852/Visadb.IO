<template>
    <nav class="navbar navbar-expand-lg navbar-light bg-light">
        <a class="navbar-brand" href="#">
            <img class="logo" src="../../assets/visa-db-brand-logo.png" alt="LOGO">
        </a>

        <button class="navbar-toggler" type="button" data-toggle="collapse" data-target="#navbarSupportedContent" aria-controls="navbarSupportedContent" aria-expanded="false" aria-label="Toggle navigation">
            <span class="navbar-toggler-icon"></span>
        </button>

        <div class="collapse navbar-collapse" id="navbarSupportedContent">

            <template v-for="(item, index) in this.navItems">

                <template v-if="item.alignRight">
                    <ul class="navbar-nav ml-auto" :key="index">
                        <app-header-item :item-text="item.text" :item-href="item.href" :item-icon-class="item.icon" />
                    </ul>
                </template>

                <template v-else>
                    <ul class="navbar-nav mr-auto" :key="index">
                        <app-header-item :item-text="item.text" :item-href="item.href" :item-icon-class="item.icon" />
                    </ul>
                </template>

            </template>

        </div>

    </nav>
</template>

<script>
    import HeaderItem from './HeaderItem.vue';

    export default {
        name: "Header",

        components: {
            appHeaderItem: HeaderItem,
        },

        data() {
            return {
                brandLogoSource: require('../../assets/visa-db-brand-logo.png'),
                navItems: [
                    {
                        text: 'Search',
                        icon: 'fas fa-search',
                        href: '#',
                        alignRight: false,
                    },
                    {
                        text: 'Ask Question',
                        icon: '',
                        href: '#',
                        alignRight: false,
                    },
                    {
                        text: 'Passport Ranking',
                        icon: 'fas fa-passport',
                        href: '#',
                        alignRight: false,
                    },
                    {
                        text: 'Partner',
                        icon: 'fas fa-hands-helping',
                        href: '#',
                        alignRight: false,
                    },
                    {
                        text: 'News',
                        icon: 'far fa-newspaper',
                        href: '#',
                        alignRight: false,
                    },
                    {
                        text: 'Contact Use',
                        icon: 'fas fa-envelope',
                        href: '#',
                        alignRight: false,
                    },
                    {
                        text: 'More',
                        icon: 'fas fa-ellipsis-h',
                        href: '#',
                        alignRight: false,
                    },
                    {
                        text: 'Login',
                        icon: 'far fa-user',
                        href: '#',
                        alignRight: true,
                    },
                    {
                        text: 'Select language',
                        icon: 'fas fa-caret-down',
                        href: '#',
                        alignRight: true,
                    },
                ]
            }
        }
    }
</script>

<style scoped>
    .logo {
        position: relative;
        width: 180px;
        height: auto;
        left: 12px;
        right: 8px;

        opacity: 0.5;
    }

    .navbar {
        padding: 0;
        margin: 0;
    }

    .bg-light {
        background-color: #0150B1 !important;
    }
</style>
