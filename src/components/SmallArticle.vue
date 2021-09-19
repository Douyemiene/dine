<template>
  <div>
    <img class="image" :src="require(`@/assets/${image}`)" />
    <div>
      <h3 class="head">{{ head }}</h3>
      <p class="body-two">
        {{ text }}
      </p>
    </div>
  </div>
</template>

<script>
export default {
  props: {
    imageTop: Boolean,
    image: String,
    head: String,
    text: String,
  },
};
</script>

<style scoped>
div {
  display: flex;
  flex-direction: column;
  align-items: center;
  padding: 0 0.25rem;
  text-align: center;
  margin-bottom: 2rem;
}

.image {
  display: block;
  width: 100%;
  height: 254px;
  margin: 0 auto;
}

div:nth-child(2) {
  padding-top: 4rem;
}

.head {
  letter-spacing: -0.4px;
}
</style>
