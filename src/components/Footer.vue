<template>
  <div class="index-footer">
    <div class="index-footer-top">
      <div class="nav-wrapper">
        <div>
          <h4>dc comics</h4>
          <nav>
            <ul>
              <li>Characters</li>
              <li>Comics</li>
              <li>Movies</li>
              <li>TV</li>
              <li>Games</li>
              <li>Videos</li>
              <li>News</li>
            </ul>
          </nav>
        </div>
        <div>
          <h4>shop</h4>
          <nav>
            <ul>
              <li>Shop DC</li>
              <li>Shop DC Collectables</li>
            </ul>
          </nav>
        </div>
        <div>
          <h4>dc</h4>
          <nav>
            <ul>
              <li>Terms Of Use</li>
              <li>Privacy policy (New)</li>
              <li>Ad Choices</li>
              <li>Advertising</li>
              <li>Jobs</li>
              <li>Subscriptions</li>
              <li>Talent Workshops</li>
              <li>Ratings</li>
              <li>Shop Help</li>
              <li>Contact Us</li>
            </ul>
          </nav>
        </div>
        <div>
          <h4>sites</h4>
          <nav>
            <ul>
              <li>DC</li>
              <li>MAD Magazine</li>
              <li>DC Kids</li>
              <li>DC Universe</li>
              <li>DC Power Visa</li>
            </ul>
          </nav>
        </div>
      </div>
      <img src="../assets/images/dc-logo-bg.png" alt="logo dc" />
    </div>
    <div class="index-footer-bottom">
      <button>sign-up now!</button>
      <div class="social-wrapper">
        <a href="#">folow us</a>
        <a href="#">
          <img src="../assets/images/footer-facebook.png" alt="facebook logo" />
        </a>
        <a href="#">
          <img src="../assets/images/footer-twitter.png" alt="twitter logo" />
        </a>
        <a href="#">
          <img src="../assets/images/footer-youtube.png" alt="youtube logo " />
        </a>
        <a href="#">
          <img
            src="../assets/images/footer-pinterest.png"
            alt="pinterest logo"
          />
        </a>
        <a href="#"
          ><img src="../assets/images/footer-periscope.png" alt="periscope" />
        </a>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "IndexFooter",
};
</script>

<style lang="scss" scooped>
div.index-footer-top {
  height: 380px;
  color: white;
  display: flex;
  background-size: cover;
  background-repeat: no-repeat;
  justify-content: space-around;
  background-image: url(../assets/images/footer-bg.jpg);
  div.nav-wrapper {
    padding: 1.5rem;
    display: flex;
    flex-wrap: wrap;
    flex-direction: column;
    div {
      display: flex;
      flex-direction: column;
      margin-bottom: 1rem;
      h4 {
        text-transform: uppercase;
        margin-bottom: 1.5rem;
      }
      nav {
        display: flex;
        flex-direction: column;
        align-items: flex-start;
        ul {
          display: flex;
          flex-direction: column;
          align-items: flex-start;
          li {
            padding: 0;
          }
        }
      }
    }
  }
  img {
    scale: 1.2;
  }
}

div.index-footer-bottom {
  z-index: 2;
  height: 97px;
  display: flex;
  position: relative;
  align-items: center;
  justify-content: space-around;
  background-color: rgb(48, 48, 48);
  button {
    color: white;
    padding: 0.5rem;
    font-weight: 600;
    text-transform: uppercase;
    background-color: transparent;
    border: 2px solid rgb(2, 130, 249);
  }
  div.social-wrapper {
    display: flex;
    align-items: center;
    justify-content: space-evenly;
    a {
      font-weight: 800;
      margin-right: 1rem;
      text-decoration: none;
      color: rgb(2, 130, 249);
      text-transform: uppercase;
    }
  }
}
</style>
