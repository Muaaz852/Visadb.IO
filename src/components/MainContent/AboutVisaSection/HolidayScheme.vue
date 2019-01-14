<template>
    <div class="row">
        <div class="col-md-6 col-sm-12">
            <span class="span-bg-red text-right">
                <slot name="holiday-scheme-text">

                </slot>
            </span>

            <h1 class="text-red">
                <slot name="holiday-scheme-heading">

                </slot>
            </h1>
        </div>

        <div class="col-md-6 col-sm-12">

            <div class="float-md-right">
                <span class="text-right span-date-time ">
                    <slot name="holiday-scheme-right-datetime">

                    </slot>
                </span>

                <button class="btn btn-outline-primary mt-3">
                    <i class="fas fa-pen"></i>
                    <slot name="holiday-scheme-right-button-text">

                    </slot>
                </button>
            </div>
        </div>
    </div>

</template>

<script>
    export default {
        name: "HolidayScheme"
    }
</script>

<style scoped>
    .span-bg-red {
        /* Holiday visa required */
        display: inline-block;
        background: #FF0935;
        padding: 2px 10px;
        font-family: 'Quicksand', cursive;
        font-style: normal;
        font-weight: bold;
        font-size: 20px;
        color: #FFFFFF;
    }

    h1 {
        width: 467px;
        height: 38px;
        padding: 5px 0;
        font-style: normal;
        font-weight: normal;
        line-height: normal;
        font-size: 30px;
        letter-spacing: 0.1em;
        text-transform: uppercase;
        color: #FF0935;
    }
    .btn {
        display: block;
        font-style: normal;
        font-weight: bold;
        font-size: 15px;
        border-radius: 0;
        padding: 10px;
    }

    .span-date-time {
        font-size: 15px;
        color: #86888C;
    }
</style>