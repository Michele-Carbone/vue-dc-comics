<template>
  <div id="jumbotron">
    <div id="content" class="">
      <div class="container">
        <h1>-->Content goes here</h1>
      </div>
    </div>
    <div id="products">
      <div class="container">
        <ul>
          <li v-for="(icon, index) in icons" :key="index">
            <img :src="icon.image" :alt="icon.text" />{{ icon.text }}
          </li>
        </ul>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "Jumbotron",
  data() {
    return {
      icons: [
        {
          image: require("@/assets/img/buy-comics-digital-comics.png"),
          text: "DIGITAL COMICS",
        },
        {
          image: require("@/assets/img/buy-comics-merchandise.png"),
          text: "DC MERCHANDISE",
        },
        {
          image: require("@/assets/img/buy-comics-subscriptions.png"),
          text: "SUBSCRIPTION",
        },
        {
          image: require("@/assets/img/buy-comics-shop-locator.png"),
          text: "COMIC SHOP LOCATOR",
        },
        {
          image: require("@/assets/img/buy-dc-power-visa.svg"),
          text: "DC POWER VISA",
        },
      ],
    };
  },
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
  height: 150px;
}

#products ul {
  display: flex;
  padding: 0;
  justify-content: space-between;
}
#products ul li img {
  width: 50px;
  vertical-align: middle;
  margin: 35px 0;
}

#products ul li {
  list-style-type: none;
  font-weight: bold;
  padding: 15px 10px;
}

#products ul li a:hover,
#products ul li a.active {
  color: red;
  border-bottom: 2px solid red;
}
</style>