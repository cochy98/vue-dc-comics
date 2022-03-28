<template>
  <main>
    <section id="main-content">
      <div class="container">
        <h1>Content goes here</h1>
      </div>
    </section>

    <section id="main-nav">
      <div class="container">
        <ul>
          <li>
            <img
              src="../assets/img/buy-comics-digital-comics.png"
              alt="Digital comics"
            />
            <p>Digital comics</p>
          </li>
          <li>
            <img
              src="../assets/img/buy-comics-merchandise.png"
              alt="Dc merchandise"
            />
            <p>Dc merchandise</p>
          </li>
          <li>
            <img
              src="../assets/img/buy-comics-subscriptions.png"
              alt="Subscription"
            />
            <p>Subscription</p>
          </li>
          <li>
            <img
              src="../assets/img/buy-comics-shop-locator.png"
              alt="Comic shop locator"
            />
            <p>Comic shop locator</p>
          </li>
          <li>
            <img
              src="../assets/img/buy-dc-power-visa.svg"
              alt="Dc power visa"
            />
            <p>Dc power visa</p>
          </li>
        </ul>
      </div>
    </section>
  </main>
</template>

<script>
export default {
  name: "IndexContent",
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
main {
  color: white;

  section#main-content {
    background-color: #1c1c1c;
    padding: 3rem 0;
  }

  section#main-nav {
    background-color: #0282f9;
  }

  section#main-nav ul {
    list-style-type: none;
    display: flex;
    justify-content: space-between;
    padding: 3rem;

    li {
      display: flex;
      align-items: center;
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
