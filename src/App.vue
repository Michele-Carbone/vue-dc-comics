<template>
  <div id="app" class="container-fluid">
    <Header />
    <Jumbotron />
    <Footer />
    <Footer_Follow />
  </div>
</template>

<script>
import Header from "@/components/Header.vue";
import Jumbotron from "@/components/Jumbotron.vue";
import Footer from "@/components/Footer.vue";
import Footer_Follow from "@/components/Footer_Follow.vue";
export default {
  name: "App",
  components: {
    Header,
    Footer,
    Jumbotron,
    Footer_Follow,
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

.container-fluid {
  width: 100%;
}

body {
  font-family: "Kurale", serif;
}
/*
img {
  max-width: 100%;
  height: auto;
}
*/
a {
  text-decoration: none;
  color: black;
}
</style>
