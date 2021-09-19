<template>
  <div id="jumbotron">
    <div id="content" class="">
      <div class="container"></div>
    </div>
    <div class="series">
      <div class="container title-series">
        <span>CURRENT SERIES</span>
        <ul>
          <li v-for="(serie, index) in series" :key="index">
            <img :src="serie.thumb" alt="" />
            <h4>{{ serie.series }}</h4>
          </li>
        </ul>
        <div class="load">
          <button>LOAD MORE</button>
        </div>
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
      series: [
        {
          thumb:
            "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2018/09/AC1000_DLX_162-001_HD_5ba13723281ab0.37845353.jpg?itok=ZsI-C5eX",
          price: "$19.99",
          series: "Action Comics",
          type: "comic book",
        },
        {
          thumb:
            "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2020/09/AV1976_01_300-001_HD_5f738f6e39ddd7.18205602.jpg?itok=VgdYdJ01",
          price: "$3.99",
          series: "American Vampire 1976",
          type: "comic book",
        },
        {
          thumb:
            "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/gn-covers/2018/08/AQMv4_UW_153-001_HD_5b7efa1745a9b8.08589135.jpg?itok=HPTtnrsb",
          price: "$16.99",
          series: "Aquaman",
          type: "graphic novel",
        },
        {
          thumb:
            "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2018/06/batgirl_v5_1_5b23e1f1124941.50950783.jpg?itok=VnrJah76",
          price: "$2.99",
          series: "Batgirl",
          type: "comic book",
        },
        {
          thumb:
            "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2018/09/BM_56_300-001_HD_5ba137a85c3bf3.33122291.jpg?itok=3FHJQYJZ",
          price: "$3.99",
          series: "Batman",
          type: "comic book",
        },
        {
          thumb:
            "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2018/09/BM_56_300-001_HD_5ba137a85c3bf3.33122291.jpg?itok=3FHJQYJZ",
          price: "$2.99",
          series: "Batman Beyond",
          type: "comic book",
        },
        {
          thumb:
            "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2019/08/BMSM_5d4361b7116261.74371456.jpg?itok=kEDR2OL8",
          price: "$3.99",
          series: "Batman/Superman",
          type: "comic book",
        },
        {
          thumb:
            "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2020/09/BMSMANN_01_300-001_HD_5f5ff17fa1d665.74704970.jpg?itok=azz5sfGk",
          price: "$4.99",
          series: "Batman/Superman Annual",
          type: "comic book",
        },
        {
          thumb:
            "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2020/09/BMTJWZ_01_300-001_HD_5f5ff2307dcb37.34652945.jpg?itok=VswVjLR8",
          price: "$5.99",
          series: "Batman: The Joker War Zone",
          type: "comic book",
        },
        {
          thumb:
            "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2020/08/cover-v2_5f40314645a734.37285065.png?itok=ImNM2QBY",
          price: "$6.99",
          series: "Batman: Three Jokers",
          type: "comic book",
        },
        {
          thumb:
            "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2020/10/BMWK_HQ_01_300-001_HD_5f7cb4945e13f6.89501032.jpg?itok=sVwALbUX",
          price: "$4.99",
          series: "Batman: White Knight Presents: Harley Quinn",
          type: "comic book",
        },
        {
          thumb:
            "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/gn-covers/2019/04/CTWv1_CC_144-001_HD_5ca5299a751963.53054221.jpg?itok=ooPaoLDq",
          price: "$16.99",
          series: "Catwoman",
          type: "graphic novel",
        },
      ],
    };
  },
};
</script>

<style>
#content {
  background-image: url("../assets/img/jumbotron.jpg");
  height: 400px;
  background-repeat: no-repeat;
  background-position: top;
  background-size: cover;
}

.series {
  background-color: rgba(0, 0, 0, 0.883);
  color: white;
  font-weight: bold;
}
.title-series {
  position: relative;
}

.series ul {
  list-style: none;
  padding: 40px 10px;
  display: flex;
  flex-wrap: wrap;
  justify-content: left;
}

.series ul li {
  flex-basis: 150px;
  text-align: center;
  min-height: 100px;
  margin: 10px 20px;
}

.series ul li img {
  width: 150px;
}

span {
  color: white;
  background-color: dodgerblue;
  padding: 5px 20px;
  position: absolute;
  margin-top: -20px;
}

.load {
  text-align: center;
}

.load button {
  color: white;
  background-color: dodgerblue;
  padding: 5px 20px;
  margin: 20px;
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