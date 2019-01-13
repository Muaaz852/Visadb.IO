<template>
  <div id="app">

    <app-header />

  </div>
</template>

<script>

import Header from './components/Header/Header.vue';

export default {
  name: 'App',
  components: {
      appHeader: Header
  },
  data () {
    return {
      //
    }
  }
}
</script>
