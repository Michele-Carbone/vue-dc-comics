<template>
  <div id="footer-follow">
    <div class="container social">
      <div class="sign-up">
        <button>SIGN-UP NOW!</button>
      </div>
      <div class="follow">
        <ul>
          <li>FOLLOW US</li>
          <li>
            <a href="#"><i class="fab fa-facebook"></i></a>
          </li>
          <li>
            <a href="#"><i class="fab fa-twitter-square"></i></a>
          </li>
          <li>
            <a href="#"><i class="fab fa-youtube-square"></i></a>
          </li>
          <li>
            <a href="#"><i class="fas fa-star"></i></a>
          </li>
          <li>
            <a href="#"><i class="fas fa-map-marker-alt"></i></a>
          </li>
        </ul>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "Footer_Follow",
};
</script>

<style>
#footer-follow {
  height: 100px;
  background-color: rgb(47, 47, 47);
  color: white;
}

.social {
  display: flex;
  justify-content: space-between;
  align-items: center;
}

.sign-up button {
  margin-top: 20px;
  padding: 10px;
  margin-left: 20px;
  border-bottom-color: 2px solid dodgerblue;
  background-color: rgb(47, 47, 47);
  color: white;
}

.follow ul {
  margin-top: 20px;
  color: dodgerblue;
  display: flex;
  padding: 0;
  justify-content: center;
}

.follow ul li a {
  padding: 15px 10px;
}

.follow ul li {
  list-style-type: none;
  font-weight: bold;
}

.follow .fab {
  font-size: 1.5rem;
  color: rgb(92, 92, 92);
  padding: 0 5px;
}

.follow .fas {
  font-size: 1.5rem;
  color: rgb(92, 92, 92);
  padding: 0 5px;
}
</style>