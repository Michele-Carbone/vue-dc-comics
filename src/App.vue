<template>
  <div id="app">
    <Header />
  </div>
</template>

<script>
import Header from "@/components/Header.vue";
export default {
  name: "App",
  components: {
    Header,
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
</style>
