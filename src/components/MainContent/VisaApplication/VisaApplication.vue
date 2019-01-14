<template>
    <div class="row mt-4">
        <div class="col-auto mt-4">

            <v-tabs
                fixed-tabs
                light
                slider-color="#0150B1"
                >

                <v-tab
                    v-for="(tab, index) in this.tabs"
                    :key="index"
                    ripple
                    class="pr-3"
                    >
                    <i :class="tab.icon" class="ma-2 tab-icon"></i>

                    <span class="tab-text">{{tab.text}}</span>

                </v-tab>

                <v-tab-item
                        v-for="pages in 4"
                        :key="pages"
                >
                    <v-card flat>
                        <v-card-text>
                            Muaaz
                        </v-card-text>
                    </v-card>
                </v-tab-item>
            </v-tabs>

        </div>
    </div>
</template>

<script>
    export default {
        name: "VisaApplication",
        props: {
            tabs: Array
        },
        data() {
            return {
                active: null,
                text: ''
            }
        },
    }
</script>

<style scoped>
    .tab-icon {
        color: #0150B1;
        font-size: 25px;
    }
    .tab-text {
        font-family: 'Quicksand', cursive;
        color: #0150B1;
        font-size: 28px;
    }
</style>