<template>
    <div>
        <slot name="nav-brand-logo">

            <a class="navbar-brand" href="#">

                <slot name="nav-item-brand-logo">

                </slot>

            </a>

        </slot>

        <ul class="nav nav-pills">
            <li class="nav-item">

                <slot name="nav-simple-item">

                </slot>

            </li>
        </ul>
        <!--<slot name="nav-login-button">-->

        <!--</slot>-->

        <!--<slot name="nav-language-select">-->

        <!--</slot>-->

    </div>
</template>

<script>

    export default {
        name: "HeaderItem",
    }

</script>

<style scoped>
    .brand-logo {
        position: absolute;
        left: 12px;
        top: 8px;

        /*background: url(../../assets/visa-db-brand-logo.png);*/
        opacity: 0.5;
    }
</style>

/* image */

position: absolute;
width: 142.33px;
height: 35px;
left: 12px;
top: 8px;

background: url(image.png);
opacity: 0.5;
