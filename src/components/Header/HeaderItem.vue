<template>

    <li class="nav-item pl-5 ml-5">
        <a class="nav-link" :href="this.itemHref">

            <i :class="this.itemIconClass">

            </i>

            {{ this.itemText }}
        </a>
    </li>

</template>

<script>

    export default {
        name: "HeaderItem",
        props: {
            itemText: String,
            itemHref: String,
            itemIconClass: String,
        }
    }

</script>

<style scoped>
    .navbar-expand-lg .navbar-nav .nav-link {
        /*padding-left: 2.5rem;*/
    }
    .navbar-light .navbar-nav .nav-link{
        color: rgb(255, 255, 255);
    }
</style>