<template>
    <div>

        <div v-for="(data, index) in this.visaProperties" :key="index" class="properties-block">
            <i :class="data.icon" class="icon-visa"></i>
            <span class="span-visa">  {{ data.text_1 }}: </span>
            <span class="span-visa-duration">{{ data.text_2 }}</span>
        </div>

    </div>
</template>

<script>
    export default {
        name: "VisaProperties",
        props: {
            visaProperties: Array,
        }
    }
</script>

<style scoped>
    .properties-block {
        color: #027BE3 !important;
        margin-bottom: 15px;
    }
    .icon-visa {
        font-size: 30px;
    }

    .span-visa {
        font-family: 'Quicksand', cursive;
        font-size: 22px;
    }

    .span-visa-duration {
        font-weight: bold;
        font-size: 22px;
    }
</style>