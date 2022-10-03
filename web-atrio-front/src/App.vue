<template>
  <Header />
  <ProgressBars />
</template>

<script>
import Header from "./components/Header.vue";
import ProgressBars from "./components/ProgressBars.vue";

export default {
  name: "App",
  components: {
    Header,
    ProgressBars,
  },
};
</script>

<style>
:root {
  /* colors */
  --color-darker: #242424;
  --color-dark: #373737;
  --color-dark-transparent: #00000029;
  --color-medium: #707070;
  --color-lighter: #ffffff;
  --color-first-quarter: #7160e8;
  --color-second-quarter: #60ade8;
  --color-third-quarter: #60e8b6;
  --color-last-quarter: #30db63;

  /* fonts */
  --font-size: 16px;
  --font-family: "Roboto", sans-serif;
}
#app {
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: var(--color-lighter);
  font-family: var(--font-family);
  font-size: var(--font-size);
  background: var(--color-darker);
  padding-top: 164px;
  height: 100vh;
}
</style>
