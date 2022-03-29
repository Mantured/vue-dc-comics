<template>
  <div class="index-header">
    <!-- img -->
    <img src="../assets/images/dc-logo.png" alt="main logo Dc" />
    <!-- nav -->
    <nav>
      <ul>
        <li v-for="(link, index) in navLinks" :key="index">
          <a
            :href="link.href"
            :class="{active: link.active}"
            @click="toggle(index)"
            >{{ link.text }}</a
          >
        </li>
      </ul>
    </nav>
  </div>
</template>

<script>
export default {
  name: "IndexHeader",
  data: function () {
    return {
      navLinks: [
        {
          text: "characters",
          href: "#",
          active: false,
        },
        {
          text: "comics",
          href: "#",
          active: false,
        },
        {
          text: "movies",
          href: "#",
          active: false,
        },
        {
          text: "tv",
          href: "#",
          active: false,
        },
        {
          text: "games",
          href: "#",
          active: false,
        },
        {
          text: "collectibles",
          href: "#",
          active: true,
        },
        {
          text: "videos",
          href: "#",
          active: false,
        },
        {
          text: "fans",
          href: "#",
          active: false,
        },
        {
          text: "news",
          href: "#",
          active: false,
        },
        {
          text: "shop",
          href: "#",
          active: false,
        },
      ],
    };
  },
  methods: {
    toggle() {
      this.active = !this.active;
      console.log(this.active);
    },
  },
};
</script>

<style lang="scss" scooped>
@import "../assets/scss/style.scss";

div.index-header {
  height: 13vh;
  display: flex;
  padding: 0.5rem;
  align-items: center;
  justify-content: space-around;
}
nav {
  ul {
    display: flex;
    align-items: center;
    justify-content: flex-end;

    li {
      padding: 0 0.7rem;
      list-style-type: none;
      a {
        color: black;
        font-weight: 600;
        text-decoration: none;
        text-transform: uppercase;
      }
    }
    li:hover a,
    li:active a,
    .active {
      padding-bottom: 5vh;
      border-bottom: 4px solid blue;
    }
  }
}
</style>
