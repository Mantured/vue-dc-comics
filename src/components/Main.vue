<template>
  <div class="index-main">
    <div class="index-main-top">
      <a href="#"> --> Content goes here </a>
    </div>
    <div class="index-main-bottom">
      <ul>
        <li>
          <a href="">digital comics</a>
        </li>
        <li>
          <a href="">dc merchandise</a>
        </li>
        <li>
          <a href="">subscription</a>
        </li>
        <li>
          <a href="">comic shop locator</a>
        </li>
        <li>
          <a href="">dc power visa</a>
        </li>
      </ul>
    </div>
  </div>
</template>

<script>
export default {
  name: "IndexMain",
};
</script>

<style lang="scss" scoped>
div.index-main {
  a {
    text-decoration: none;
    color: white;
    font-size: 1.5rem;
  }
}

div.index-main-top {
  height: 120px;
  display: flex;
  align-items: center;
  justify-content: center;
  background-color: black;
}

div.index-main-bottom {
  display: flex;
  height: 200px;
  align-items: center;
  justify-content: space-around;
  background-color: rgb(2, 130, 249);
  ul {
    li {
      display: inline;
      padding: 0 0.7rem;
      list-style-type: none;
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
