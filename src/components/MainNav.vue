<template>
  <section id="main-nav">
    <div class="container">
      <ul>
        <li v-for="(element, index) in mainNavLinks" :key="index">
          <a :href="element.url">
            <img :src="element.path" :alt="element.text" />
            <p>{{ element.text }}</p>
          </a>
        </li>
      </ul>
    </div>
  </section>
</template>
<script>
export default {
  name: "MainNav",
  data: function () {
    return {
      mainNavLinks: [
        {
          text: "Digital comics",
          path: require("../assets/img/buy-comics-digital-comics.png"),
          url: "#",
        },
        {
          text: "Dc merchandise",
          path: require("../assets/img/buy-comics-merchandise.png"),
          url: "#",
        },
        {
          text: "Subscription",
          path: require("../assets/img/buy-comics-subscriptions.png"),
          url: "#",
        },
        {
          text: "Comic shop locator",
          path: require("../assets/img/buy-comics-shop-locator.png"),
          url: "#",
        },
        {
          text: "Dc power visa",
          path: require("../assets/img/buy-dc-power-visa.svg"),
          url: "#",
        },
      ],
    };
  },
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
section#main-nav {
  background-color: #0282f9;

  ul {
    list-style-type: none;
    display: flex;
    justify-content: space-between;
    padding: 3rem;

    li a {
      display: flex;
      align-items: center;
      color: white;
      text-decoration: none;
      text-transform: uppercase;

      img {
        width: 55px;
        height: 55px;
        margin-right: 1rem;
        object-fit: contain;
      }
    }
  }
}
</style>
