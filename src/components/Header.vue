<template>
  <div id="log" class="container">
    <div id="logo" class="col">
      <img src="@/assets/img/dc-logo.png" alt="" />
    </div>
    <nav class="nav">
      <ul>
        <li v-for="(link, index) in links" :key="index">
          <a :href="link.url" :class="{ active: link.current }">{{
            link.text
          }}</a>
        </li>
      </ul>
    </nav>
  </div>
</template>

<script>
export default {
  name: "Header",
  data() {
    return {
      links: [
        {
          text: "Characters",
          url: "#",
          current: false,
        },
        {
          text: "Comics",
          url: "#",
          current: true,
        },
        {
          text: "Movies",
          url: "#",
          current: false,
        },
        {
          text: "TV",
          url: "#",
          current: false,
        },
        {
          text: "Games",
          url: "#",
          current: false,
        },
        {
          text: "Collectibles",
          url: "#",
          current: false,
        },
        {
          text: "Videos",
          url: "#",
          current: false,
        },
        {
          text: "Fans",
          url: "#",
          current: false,
        },
        {
          text: "News",
          url: "#",
          current: false,
        },
        {
          text: "Shop",
          url: "#",
          current: false,
        },
      ],
    };
  },
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

/*//verificare l istallazione di scss
nav{
  ul {
    display: flex;
    padding: 0;
    justify-content: center;
    li {
      list-style-type: none;
      font-weight: bold;
      a {
        padding: 15px 10px;
        &:hover,    //uso la & al posto della a per innestare
        &.active {
          color: dodgerblue;
          border-bottom: 2px solid dodgerblue;
          }
        }
    }
  }
}
*/
</style>