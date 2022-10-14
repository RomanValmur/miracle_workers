<template>
  <div id="app">
    <hints-block/>
  </div>
</template>

<script>
import HintsBlock from './components/HintsBlock.vue';

export default {
  name: 'App',
  components: {
    HintsBlock,
  },
}
</script>

<style>
body {
  margin: 0;
}
@font-face {
  font-family: 'Futura';
  src: local('Futura'),
    url('./assets/fonts/futura-bold.woff2') format('woff2');
  font-style: 700; 
  font-weight: bold;
}

@font-face {
  font-family: 'Kinopoisk';
  src: local('Kinopoisk'),
  url('./assets/fonts/kinopoisk-light.woff2') format('woff2');
  font-style: normal;
  font-weight: 300;
}

@font-face {
  font-family: 'Kinopoisk';
  src: local('Kinopoisk'),
  url('./assets/fonts/kinopoisk-regular.woff2') format('woff2');
  font-style: normal;
  font-weight: 400;
}

@font-face {
  font-family: 'Kinopoisk';
  src: local('Kinopoisk'),
  url('./assets/fonts/kinopoisk-medium.woff2') format('woff2');
  font-style: normal;
  font-weight: 500;
}

@font-face {
  font-family: 'Kinopoisk';
  src: local('Kinopoisk'),
  url('./assets/fonts/kinopoisk-semibold.woff2') format('woff2');
  font-style: normal;
  font-weight: 600;
}

@font-face {
  font-family: 'Kinopoisk';
  src: local('Kinopoisk'),
  url('./assets/fonts/kinopoisk-bold.woff2') format('woff2');
  font-style: normal;
  font-weight: 700;
}
</style>