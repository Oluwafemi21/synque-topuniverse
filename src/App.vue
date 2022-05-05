<template>
  <main>
    <main-sidebar />
    <faq-section />
  </main>
</template>

<script>
import MainSidebar from "@/components/Sidebar.vue";
import FaqSection from "./components/FaqSection.vue";
export default {
  name: "App",
  components: {
    "main-sidebar": MainSidebar,
    FaqSection,
  },
};
</script>

<style>
@font-face {
  font-family: Metropolis;
  src: url(@/assets/fonts/Metropolis-Regular.otf);
  font-weight: 400;
}

@font-face {
  font-family: Metropolis;
  src: url(@/assets/fonts/Metropolis-SemiBold.otf);
  font-weight: 500;
}

@font-face {
  font-family: Metropolis;
  src: url(@/assets/fonts/Metropolis-Bold.otf);
  font-weight: 700;
}

:root {
  --purple: #391d49;
  --yellow: #ffbd69;
  --white: #fcfcfc;
  --black: #121212;
}

/* CSS RESET */

* {
  padding: 0;
  margin: 0;
  box-sizing: border-box;
  font-family: Metropolis, sans-serif;
}

html {
  font-size: 10px;
}

#app {
  height: 100vh;
  width: 100vw;
}

main {
  height: 100%;
  width: 100%;
  display: flex;
}

a {
  text-decoration: none;
  color: inherit;
}

li {
  list-style-type: none;
}

button {
  cursor: pointer;
}
</style>
