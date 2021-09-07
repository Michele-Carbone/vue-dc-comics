<template>
  <div id="footer" class="">
    <div class="container container-bg">
      <div class="dc-comics">
        <h3>DC COMICS</h3>
        <ul>
          <li><a href="#">CHARACTERS</a></li>
          <li><a href="#">COMICS</a></li>
          <li><a href="#">MOVIES</a></li>
          <li><a href="#">TV</a></li>
          <li><a href="#">GAMES</a></li>
          <li><a href="#">COLLECTIBLES</a></li>
          <li><a href="#">VIDEOS</a></li>
          <li><a href="#">FANS</a></li>
          <li><a href="#">NEWS</a></li>
          <li><a href="#">SHOP</a></li>
        </ul>
        <h3>SHOP</h3>
        <ul>
          <li><a href="#">Shop DC</a></li>
          <li><a href="#">Shop DC Collection</a></li>
        </ul>
      </div>
      <div class="dc">
        <h3>DC</h3>
        <ul>
          <li><a href="#">Terms Of Use</a></li>
          <li><a href="#">Privacy policy (New)</a></li>
          <li><a href="#">Ad Choices</a></li>
          <li><a href="#">Advertising</a></li>
          <li><a href="#">Jobs</a></li>
          <li><a href="#">Subscriptions</a></li>
          <li><a href="#">Talent Workshops</a></li>
          <li><a href="#">CPSC Certificates</a></li>
          <li><a href="#">Ratings</a></li>
          <li><a href="#">Shop Help</a></li>
          <li><a href="#">Contact Us</a></li>
        </ul>
      </div>
      <div class="sites">
        <h3>SITES</h3>
        <ul>
          <li><a href="#">DC</a></li>
          <li><a href="#">MAD Magazine</a></li>
          <li><a href="#">DC Kids</a></li>
          <li><a href="#">DC Universe</a></li>
          <li><a href="#">DC Power Visa</a></li>
        </ul>
      </div>
      <div class="dc-logo-bg">
        <img src="@/assets/img/dc-logo-bg.png" alt="" />
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "Footer",
};
</script>

<style scoped>
#footer {
  background-image: url("../assets/img/footer-bg.jpg");
  height: 600px;
  background-repeat: no-repeat;
  background-position: center;
  background-size: cover;
}

h3 {
  color: white;
}

#footer ul li {
  list-style-type: none;
  font-weight: bold;
}

#footer ul li a {
  list-style-type: none;
  font-weight: bold;
  color: grey;
}

.dc-comics,
.dc,
.sites {
  float: left;
  margin: 20px;
}
</style>