<script>
import AppHeader from './components/AppHeader.vue';
import AppMain from './components/AppMain.vue';
import AppFooter from './components/AppFooter.vue';

export default {
  data() {
    return {
    }
  },
  components: { AppHeader, AppMain, AppFooter, }
}
</script>


<template>
  <!-- Header-->
  <AppHeader />

  <!-- Main -->
  <AppMain />

  <!-- Footer -->
  <AppFooter />
</template>

<style>
/* CSS Reset */
* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}

/* General */
body {
  font-family: 'Open Sans', 'Open Sans Condensed', sans-serif;
  background-color: #0E0E0E;
  margin: 45px 0;
}

img {
  height: auto;
  max-width: 100%;
}

a {
  text-decoration: none;
}

ul {
  list-style-type: none;
}

/* Utilities */
.container {
  margin: 0 auto;
  max-width: 1200px;
}
</style>
