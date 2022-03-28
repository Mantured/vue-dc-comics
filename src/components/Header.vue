<template>
  <div class="index-header">
    <!-- img -->
    <img src="../assets/images/dc-logo.png" alt="main logo Dc" />
    <!-- nav -->
    <nav>
      <ul>
        <li>
          <a href="#">characters</a>
        </li>
        <li>
          <a href="#" class="active">comics</a>
        </li>
        <li>
          <a href="#">movies</a>
        </li>
        <li>
          <a href="#">tv</a>
        </li>
        <li>
          <a href="#">games</a>
        </li>
        <li>
          <a href="#">collectibles</a>
        </li>
        <li>
          <a href="#">videos</a>
        </li>
        <li>
          <a href="#">fans</a>
        </li>
        <li>
          <a href="#">news</a>
        </li>
        <li>
          <a href="#">shop</a>
        </li>
      </ul>
    </nav>
  </div>
</template>

<script>
export default {
  name: "IndexHeader",
};
</script>

<style lang="scss" scooped>
div.index-header {
  display: flex;
  padding: 0.5rem;
  align-items: center;
  justify-content: space-around;
}
nav {
  width: 65%;

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
    a.active {
      padding-bottom: 46px;
      border-bottom: 4px solid blue;
    }
  }
}
</style>
