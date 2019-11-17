<template>
  <div class="card">
    <b-card class="card-layanan">
      <div class="border-image img-layanan">
        <b-img
          class="m-auto"
          center
          :src="require('@/assets/images/'+images+'.svg')"
          rounded="circle"
          alt="Center image"
          width="68"
          height="68"
        ></b-img>
      </div>
      <b-card-text class="text-center mt-3">
        <b class="text-uppercase">{{title}}</b>
      </b-card-text>
      <b-card-text class="text-center mt-3">{{subtitle}}</b-card-text>
    </b-card>
  </div>
</template>

<script>
export default {
  name: "Card",
  props: {
    images: String,
    title: String,
    subtitle: String
  },
  methods: {}
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
.card {
  height: 50vh;
  width: 100%;
  box-shadow: 4px 0px rgba(243, 241, 241, 0.1), 0px 4px rgba(243, 241, 241, 0.1),
    0px -4px rgba(243, 241, 241, 0.1), -4px 0px rgba(243, 241, 241, 0.1);
}

.border-image {
  box-shadow: inset 0 2px 0px rgba(243, 241, 241, 0.2),
    0 2px 3px rgba(136, 136, 136, 0.2), 0 3px 9px rgba(136, 136, 136, 0.2);
  border-radius: 50%;
  width: 12vh;
  height: 12vh;
  margin: 0 auto;
  padding: 3px 4px;
}

.m-auto {
  margin: 0 auto;
}
</style>
