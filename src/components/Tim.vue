<template>
  <div class="cardTim">
    <b-card
      :img-src="require('@/assets/images/default.jpg')"
      img-alt="Card image"
      img-left
      class="mb-3"
      img-width="180"
      img-height="224"
    >
      <b-card-text>
        <b>{{name}}</b>
        <br />
        <p>{{job}}</p>
      </b-card-text>
      <b-card-text>{{overview}}</b-card-text>
      <b-img
        class="mr-2"
        :src="require('@/assets/images/facebook-logo.svg')"
        fluid
        alt="Fluid image"
        width="15"
        height="15"
      ></b-img>
      <b-img
        class="mr-2"
        :src="require('@/assets/images/instagram (1).svg')"
        fluid
        alt="Fluid image"
        width="15"
        height="15"
      ></b-img>
      <b-img
        class="mr-2"
        :src="require('@/assets/images/linkedin (1).svg')"
        fluid
        alt="Fluid image"
        width="15"
        height="15"
      ></b-img>
    </b-card>
  </div>
</template>

<script>
export default {
  name: "Tim",
  props: {
    images: String,
    name: String,
    job: String,
    overview: String
  }
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
.cardTim {
  height: 35vh;
  width: 100%;
}
</style>
