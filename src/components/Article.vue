<template>
  <div>
    <img
      :class="imageTop ? 'imageTop' : 'image'"
      :src="require(`@/assets/${image}`)"
    />
    <div>
      <h2 class="head">{{ head }}</h2>
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
  position: relative;
  top: -3rem;
  flex-direction: column;
  align-items: center;
  padding: 0 0.25rem;
  text-align: center;
}
.imageTop {
  /* position: absolute;
  top: -60px; */
  height: 400px;
}

.image {
  display: block;
  height: 400px;
  margin: 0 auto;
}

div:nth-child(2) {
  padding-top: 4rem;
}

.head {
  font-size: 32px;
  line-height: 40px;
  letter-spacing: -0.4px;
}

section:nth-child(3) {
  background: black;
}
</style>
