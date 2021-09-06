<template>
  <div id="log" class="container">
    <div id="logo" class="col">
      <img src="@/assets/img/dc-logo.png" alt="" />
    </div>
    <nav class="col">
      <ul>
        <li><a href="#">CHARACTERS</a></li>
        <li><a href="#" class="active">COMICS</a></li>
        <li><a href="#">MOVIES</a></li>
        <li><a href="#">TV</a></li>
        <li><a href="#">GAMES</a></li>
        <li><a href="#">COLLECTIBLES</a></li>
        <li><a href="#">VIDEOS</a></li>
        <li><a href="#">FANS</a></li>
        <li><a href="#">NEWS</a></li>
        <li><a href="#">SHOP</a></li>
      </ul>
    </nav>
  </div>
</template>

<script>
export default {
  name: "Header",
};
</script>

<style>
.container {
  max-width: 1200px;
  margin: 0 auto;
}

#log {
  margin-top: 20px;
  display: flex;
  justify-content: space-between;
  align-items: center;
}

ul {
  display: flex;
  padding: 0;
  justify-content: center;
}

ul li {
  list-style-type: none;
  font-weight: bold;
}

ul li a {
  padding: 15px;
}

ul li a:hover,
ul li a.active {
  color: blue;
}

.col {
  float: left;
}
</style>