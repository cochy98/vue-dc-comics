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
          <li
            v-for="(element, index) in headerLinks"
            :key="index"
            :class="{ active: element.current }"
          >
            <a :href="element.url">{{ element.text }}</a>
          </li>
        </ul>
      </nav>
    </div>
  </header>
</template>

<script>
export default {
  name: "IndexHeader",
  data: function () {
    return {
      headerLinks: [
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
          text: "Tv",
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
      border-bottom: 3px solid #0282f9;
    }

    li.active a {
      color: #0282f9;
    }
  }
}
</style>
