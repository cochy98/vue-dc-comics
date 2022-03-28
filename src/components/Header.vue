<template>
  <header>
    <div class="container">
      <nav>
        <img
          src="../assets/img/dc-logo.png"
          class="header-logo"
          alt="DC Logo"
        />
        <ul>
          <li><a href="#">Characters</a></li>
          <li class="active"><a href="#">Comics</a></li>
          <li><a href="#">Movies</a></li>
          <li><a href="#">Tv</a></li>
          <li><a href="#">Games</a></li>
          <li><a href="#">Collectibles</a></li>
          <li><a href="#">Videos</a></li>
          <li><a href="#">Fans</a></li>
          <li><a href="#">News</a></li>
          <li><a href="#">Shop</a></li>
        </ul>
      </nav>
    </div>
  </header>
</template>

<script>
export default {
  name: "IndexHeader",
  data: function () {
    return {};
  },
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
nav {
  display: flex;
  justify-content: space-between;
  align-items: center;

  .header-logo {
    width: 70px;
  }

  ul {
    list-style-type: none;

    li {
      display: inline-block;
      height: 100px;
      line-height: 100px;
      margin: 0 1rem;
      font-weight: 600;
      font-size: 0.8rem;
      text-transform: uppercase;

      a {
        text-decoration: none;
        color: #2c3136;
      }
    }

    li.active {
      border-bottom: 2px solid #0282f9;
    }

    li.active a {
      color: #0282f9;
    }
  }
}
</style>
