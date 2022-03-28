<template>
  <footer>
    <section id="footer-top">
      <div class="container">
        <div class="col-left">
          <div class="col">
            <h6>Dc comics</h6>
            <ul>
              <li><a href="#">Characters</a></li>
              <li><a href="#">Comics</a></li>
              <li><a href="#">Movies</a></li>
              <li><a href="#">TV</a></li>
              <li><a href="#">Games</a></li>
              <li><a href="#">Videos</a></li>
              <li><a href="#">News</a></li>
            </ul>
            <h6>Shop</h6>
            <ul>
              <li><a href="#">Shop DC</a></li>
              <li><a href="#">Shop DC Collectibles</a></li>
            </ul>
          </div>
          <div class="col">
            <h6>Dc</h6>
            <ul>
              <li><a href="#">Characters</a></li>
              <li><a href="#">Comics</a></li>
              <li><a href="#">Movies</a></li>
              <li><a href="#">Tv</a></li>
              <li><a href="#">Games</a></li>
              <li><a href="#">Videos</a></li>
              <li><a href="#">News</a></li>
            </ul>
          </div>
          <div class="col">
            <h6>Sites</h6>
            <ul>
              <li><a href="#">Characters</a></li>
              <li><a href="#">Comics</a></li>
              <li><a href="#">Movies</a></li>
              <li><a href="#">Tv</a></li>
              <li><a href="#">Games</a></li>
              <li><a href="#">Videos</a></li>
              <li><a href="#">News</a></li>
            </ul>
          </div>
        </div>
        <div class="col-right">
          <img src="../assets/img/dc-logo-bg.png" alt="Dc logo" />
        </div>
      </div>
    </section>
    <section id="footer-bottom">
      <div class="container">
        <a class="action-btn">Sign-Up now!</a>

        <ul class="social-links">
          <li><a href="#">Follow us</a></li>
          <li>
            <a href="#"
              ><img src="../assets/img/footer-facebook.png" alt="fb logo"
            /></a>
          </li>
          <li>
            <a href="#"
              ><img src="../assets/img/footer-twitter.png" alt="twitter logo"
            /></a>
          </li>
          <li>
            <a href="#"
              ><img src="../assets/img/footer-youtube.png" alt="youtube logo"
            /></a>
          </li>
          <li>
            <a href="#"
              ><img
                src="../assets/img/footer-pinterest.png"
                alt="pinterest logo"
            /></a>
          </li>
          <li>
            <a href="#"
              ><img
                src="../assets/img/footer-periscope.png"
                alt="periscope logo"
            /></a>
          </li>
        </ul>
      </div>
    </section>
  </footer>
</template>

<script>
export default {
  name: "IndexFooter",
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
h6 {
  font-size: 1.2rem;
  padding: 1.1rem 0;
  text-transform: uppercase;
}

section#footer-top {
  background-image: url("../assets/img/footer-bg.jpg");
  background-size: cover;
  color: white;

  .container {
    display: flex;
    justify-content: space-between;
    align-items: center;

    .col-left {
      display: flex;
    }

    .col-left,
    .col-right {
      flex-basis: 50%;
    }

    ul {
      list-style-type: none;
      padding-right: 2rem;

      a {
        text-decoration: none;
        font-size: 0.8rem;
        color: rgb(184, 180, 180);
        padding-bottom: 0.5rem;
      }
    }

    .col-right img {
      width: 450px;
      height: 350px;
      object-fit: cover;
    }
  }
}

section#footer-bottom {
  background-color: #303030;
}

section#footer-bottom .container {
  display: flex;
  justify-content: space-between;
  align-items: center;

  a {
    text-transform: uppercase;
    text-decoration: none;
    font-weight: bold;
  }

  a.action-btn {
    padding: 0.8rem;
    border: 2px solid #0282f9;
    color: white;
  }

  ul.social-links {
    list-style-type: none;
    display: flex;
    align-items: center;

    li {
      padding: 2rem 0.8rem;

      a {
        color: #0282f9;
      }
    }
  }
}
</style>
