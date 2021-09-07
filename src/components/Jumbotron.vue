<template>
  <div id="jumbotron">
    <div id="content" class="">
      <div class="container">
        <h1>-->Content goes here</h1>
      </div>
    </div>
    <div id="products"></div>
  </div>
</template>

<script>
export default {
  name: "Jumbotron",
};
</script>

<style>
#content {
  background-color: black;
  color: white;
  height: 100px;
  display: flex;
  align-items: center;
}

h1 {
  margin-left: -600px;
}

#products {
  background-color: dodgerblue;
  color: white;
  height: 100px;
}
</style>