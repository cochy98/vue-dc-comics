<template>
  <div class="card-box">
    <img :src="cardElement.thumb" :alt="cardElement.type" class="card-image" />
    <h6 class="card-description">{{ cardElement.series }}</h6>
  </div>
</template>

<script>
export default {
  name: "ContentCard",
  props: ["cardElement"],
};
</script>

<style lang="scss" scoped>
div.card-box {
  width: 200px;
  margin: 0.5rem;
  text-transform: uppercase;

  img.card-image {
    width: 100%;
    height: 200px;
    object-fit: cover;
    object-position: top;
  }

  .card-description {
    padding: 0.8rem 0 1.2rem;
    font-size: 0.8rem;
    font-weight: 500;
  }
}
</style>
