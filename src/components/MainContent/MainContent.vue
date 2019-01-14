<template>
    <div class="container">

        <app-holiday-scheme>
            <div slot="holiday-scheme-text">
                {{ this.holidayScheme.text }}
            </div>

            <div slot="holiday-scheme-heading">
            {{  this.holidayScheme.heading }}
            </div>

            <div slot="holiday-scheme-right-datetime">
                {{  this.holidayScheme.datetime }}
            </div>

            <span slot="holiday-scheme-right-button-text">
                {{  this.holidayScheme.btnText }}
            </span>

        </app-holiday-scheme>

        <app-about-visa />

        <app-visa-application :tabs="this.visaApplication.tabs"/>

    </div>
</template>

<script>
    import HolidayScheme from './AboutVisaSection/HolidayScheme.vue';
    import AboutVisa from './AboutVisaSection/AboutVisa.vue';
    import VisaApplication from './VisaApplication/VisaApplication.vue';

    export default {
        name: "MainContent",
        components: {
            appHolidayScheme: HolidayScheme,
            appAboutVisa: AboutVisa,
            appVisaApplication: VisaApplication,
        },
        data() {
            return {
                holidayScheme: {
                    text: 'Holiday visa required',
                    heading: 'WORKING HOLIDAY SCHEME',
                    datetime: 'Last Updated 2018-11-26 8:54pm',
                    btnText: 'Add or correct info',
                },

                visaApplication: {
                    tabs: [
                        {
                            icon: 'fas fa-check-double',
                            text: 'ELIGIBILITY',
                        },
                        {
                            icon: 'fas fa-file-alt',
                            text: 'DOCUMENTS',
                        },
                        {
                            icon: 'fas fa-list-ol',
                            text: 'FORMS',
                        },
                        {
                            icon: 'fas fa-clipboard-check',
                            text: 'APPLY',
                        },
                    ]
                }
            }
        }
    }
</script>

<style scoped>

</style>