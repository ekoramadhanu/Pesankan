<template>
  <div class="card">
    <b-card>
      <b-img center :src="images" rounded="circle" alt="Center image"></b-img>
      <b-card-text class="text-center mt-2">
        <b>{{name}}</b>
        <br />
        <p>{{job}}</p>
      </b-card-text>
      <b-card-text class="text-center mt-1">{{overview}}</b-card-text>
      <b-card-text class="text-center mt-1"></b-card-text>
    </b-card>
  </div>
</template>

<script>
export default {
  name: "Testimoni",
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
</style>
