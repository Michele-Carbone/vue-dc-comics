<template>
  <div id="log" class="container">
    <div id="logo" class="col">
      <img src="@/assets/img/dc-logo.png" alt="" />
    </div>
    <nav class="nav">
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
#log {
  margin-top: 20px;
  display: flex;
  justify-content: space-between;
  align-items: center;
}

nav ul {
  display: flex;
  padding: 0;
  justify-content: center;
}

nav ul li a {
  padding: 15px 10px;
}

nav ul li {
  list-style-type: none;
  font-weight: bold;
}

nav ul li a:hover,
nav ul li a.active {
  color: dodgerblue;
  border-bottom: 2px solid dodgerblue;
}
</style>