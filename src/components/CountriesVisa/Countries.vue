<template>
    <div class="container-fluid my-container">
        <div class="container text-center ">
            <span>
                <img class="country-flag" :src="this.countriesAvailable[0].flagIcon" />
                <label class="country-name" > {{ this.countriesAvailable[0].countryName }}</label>

                <img src="../../assets/plane.svg" />

                <span class="holiday-visa">
                    <span>Holiday</span> Visa
                </span>

                <span class="cross-sign float-right">
                    &times;
                </span>

                <label class="country-name" > {{ this.countriesAvailable[1].countryName }}</label>
                <img class="country-flag" :src="this.countriesAvailable[1].flagIcon" />

            </span>
        </div>
    </div>
</template>

<script>

    export default {
        name: "Countries",
        data() {
            return {
                countriesAvailable: [
                    {
                        countryName: 'Canada',
                        flagIcon: 'https://lipis.github.io/flag-icon-css/flags/4x3/ca.svg',
                    },

                    {
                        countryName: 'South Korea',
                        flagIcon: 'https://lipis.github.io/flag-icon-css/flags/4x3/kr.svg',
                    },
                ]
            }
        }
    }
</script>

<style scoped>
    .my-container {
        background-color: #E5E5E5;
    }

    .country-name {
        color: #86888C;
        text-decoration: underline;
        font-family: 'Quicksand', cursive;
        font-style: normal;
        font-weight: normal;
        /*line-height: normal;*/
        font-size: 20px;
        margin: 0 10px;
    }

    .country-flag {
        width: 50px;
        height: auto;
        margin: 0 10px;
    }

    .holiday-visa {
        margin: 0 10px;
        background: #fff;
        color: #0150B1;
        padding: 5px;
        font-size: large;
    }

    .holiday-visa span {
        font-weight: bold;
    }

    .cross-sign {
        font-size: 30px;
        margin-top: -7px;
    }
</style>

/* Vector */

position: absolute;
width: 23.63px;
height: 24.27px;
left: calc(50% - 23.63px/2 - 78.3px);
top: calc(50% - 24.27px/2 - 998.37px);

background: #0150B1;
transform: matrix(0.71, 0.82, -0.61, 0.71, 0, 0);
