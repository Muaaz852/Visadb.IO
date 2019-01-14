<template>
  <div id="app">

    <app-header />
    <app-countries />
    <app-main-content />

  </div>
</template>

<script>

import Header from './components/Header/Header.vue';
import CountriesAvailable from './components/CountriesVisa/Countries';
import MainContent from './components/MainContent/MainContent.vue';

export default {
  name: 'App',
  components: {
      appHeader: Header,
      appCountries: CountriesAvailable,
      appMainContent: MainContent,
  },
  data () {
    return {
      //
    }
  }
}
</script>
