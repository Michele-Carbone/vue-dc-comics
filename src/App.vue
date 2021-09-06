<template>
  <div id="app">
    <Header />
    <Footer />
  </div>
</template>

<script>
import Header from "@/components/Header.vue";
import Footer from "@/components/Footer.vue";

export default {
  name: "App",
  components: {
    Header,
    Footer,
  },
};
</script>

<style>
/*GENERICS*/
* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}

/* UTILS*/
.container {
  max-width: 1200px;
  margin: 0 auto;
}

body {
  font-family: "Kurale", serif;
}

img {
  max-width: 100%;
  height: auto;
}

a {
  text-decoration: none;
  color: black;
}
</style>
