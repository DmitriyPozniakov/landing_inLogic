<template>
  <the-header></the-header>
  <main-content></main-content>
  <the-footer></the-footer>
</template>

<script>
import TheHeader from './components/TheHeader.vue';
import MainContent from './components/MainContent.vue';
import TheFooter from './components/TheFooter.vue';
export default {
  components: { TheHeader, MainContent, TheFooter },
}
</script>

<style>
@font-face {
  font-family: 'Gilroy-600';
  src: url('../src/assets/fonts/Gilroy-SemiBold.ttf') format('truetype');
  font-weight: normal;
  font-style: normal;
}

@font-face {
  font-family: 'Gilroy-500';
  src: url('../src/assets/fonts/Gilroy-Medium.ttf') format('truetype');
  font-weight: normal;
  font-style: normal;
}

@font-face {
  font-family: 'Gilroy-300';
  src: url('../src/assets/fonts/Gilroy-Light.ttf') format('truetype');
  font-weight: normal;
  font-style: normal;
}


@font-face {
  font-family: 'Libre Baskerville';
  src: url('../src/assets/fonts/LibreBaskerville-Italic.ttf');
  font-weight: normal;
  font-style: normal;
}

* {
  padding: 0;
  margin: 0;
  box-sizing: border-box;
}

html {
  font-size: 62.5%;
}


::-webkit-scrollbar {
  display: none;
}

.special-text {
  font-family: 'Libre Baskerville';
  font-weight: 400;
}

button {
  cursor: pointer;
}

li {
  list-style-type: none;
}

a {
  text-decoration: none;
}
</style>