<template>
    <div class="row about-visa mt-3">
        <div class="col mt-3">
            <h3 class="holiday-scheme-heading">
                About this visa
            </h3>
            <p class="visa-text" v-html="this.visaText">
            </p>

        </div>

        <!--Vuetify MAGIC............-->
        <!--Vertical Line-->
        <v-divider
            class="mx-3"
            inset
            vertical
            ></v-divider>

        <!--<div class="col-md-auto float-right vertical-line mt-4">-->
        <!--</div>-->

        <div class="col col-lg-3 mt-4">

            <app-visa-properties :visa-properties="this.visaProperties" />

        </div>

    </div>
</template>

<script>
    import VisaProperties from './VisaProperties.vue';

    export default {
        name: "AboutVisa",

        components: {
            appVisaProperties: VisaProperties
        },

        data () {
            return {
                visaText: "You can enjoy holidays in the Republic of Korea by applying Working Holiday Visa at the embassy of the republic of Korea. Working Holiday Visa allows <strong>young people to travel and work</strong> in the Republic of Korea for <strong>12 months (maximum)</strong>. The main purpose of this program is to enable the young people to have an extended holiday while supplementing necessary funds with short-term work in the Republic of Korea.\n",
                visaProperties: [
                    {
                        icon: 'fas fa-calendar-alt',
                        text_1: 'DURATION',
                        text_2: '12 MONTHS',
                    },
                    {
                        icon: 'fas fa-money-bill-alt',
                        text_1: 'FEES',
                        text_2: '$90 VISA',
                    },
                    {
                        icon: 'fas fa-puzzle-piece',
                        text_1: 'COMPLEXITY',
                        text_2: 'VERY-LOW',
                    },
                ]
            }
        }
    }
</script>

<style scoped>
    .about-visa {
        border: 1px solid #C4C4C4;
    }

    .holiday-scheme-heading {
        color: #0150B1 !important;
    }

    .visa-text{
        font-family: 'Quicksand', cursive;
        font-size: 16px;
    }
</style>