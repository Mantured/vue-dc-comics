<template>
  <div class="index-main">
    <div id="jumbotron">
      <button class="my-btn">Current Series</button>
    </div>

    <div class="index-main-top">
      <Product
        v-for="(comic, index) in comics"
        :key="index"
        :comicSrc="comic.thumb"
        :comicSeries="comic.series"
      />
      <button class="my-btn">load more</button>
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
import Product from "./Product.vue";

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
      comics: [
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
  components: {
    Product,
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

#jumbotron {
  height: 40vh;
  background-image: url(../assets/images/jumbotron.jpg);
  background-size: cover;
  position: relative;
  .my-btn {
    position: absolute;
    top: 95%;
    left: 8%;
  }
}

div.index-main-top {
  /* height: 15vh; */
  display: flex;
  flex-wrap: wrap;
  padding: 2rem 8rem;
  text-align: center;
  justify-content: center;
  /*   align-items: center;
  justify-content: center; */
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
