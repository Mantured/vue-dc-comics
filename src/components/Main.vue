<template>
  <div class="index-main">
    <div class="index-main-top">
      <a href="#"> --> Content goes here </a>
    </div>
    <div class="index-main-bottom">
      <ul>
        <li v-for="(links, index) in mainLinks" :key="index">
          <img :src="require(`@/assets/images/${links.img}`)" />
          <a :href="links.href">{{ links.text }}</a>
        </li>
      </ul>
    </div>
  </div>
</template>

<script>
export default {
  name: "IndexMain",
  data: function () {
    return {
      mainLinks: [
        {
          text: "digital comics",
          href: "#",
          img: "buy-comics-digital-comics.png",
        },
        {
          text: "dc merchandise",
          href: "#",
          img: "buy-comics-merchandise.png",
        },
        {
          text: "subscription",
          href: "#",
          img: "buy-comics-subscriptions.png",
        },
        {
          text: "comic shop locator",
          href: "#",
          img: "buy-comics-shop-locator.png",
        },
        {
          text: "dc power visa",
          href: "#",
          img: "buy-dc-power-visa.svg",
        },
      ],
    };
  },
};
</script>

<style lang="scss" scoped>
div.index-main {
  a {
    text-decoration: none;
    color: white;
    font-size: 1rem;
  }
}

div.index-main-top {
  height: 15vh;
  display: flex;
  align-items: center;
  justify-content: center;
  background-color: black;
}

div.index-main-bottom {
  display: flex;
  height: 20vh;
  align-items: center;
  justify-content: space-around;
  background-color: rgb(2, 130, 249);
  ul {
    li {
      display: inline;
      padding: 0 0.7rem;
      list-style-type: none;
      img {
        width: 60px;
        height: 60px;
        margin-right: 1rem;
        vertical-align: middle;
      }
      a {
        text-transform: uppercase;
      }
    }
    /*     li:after{
      content: ;
    } */
  }
}
</style>
