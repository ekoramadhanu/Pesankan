<template>
  <div id="navbar">
    <b-navbar
      class="grey-1 pl-5 pr-5"
      toggleable="lg"
      variant="info"
      id="navbar"
      v-if="fixedTop"
      fixed="top"
      v-on:scroll="handleScroll"
    >
      <b-navbar-brand href="#">
        <b-img
          :src="require('@/assets/images/logo-pesankan.png')"
          fluid
          alt="Responsive image"
          width="148"
          height="35"
          gravity="faces"
          crop="fill"
        ></b-img>
      </b-navbar-brand>

      <b-navbar-toggle target="nav-collapse"></b-navbar-toggle>

      <b-collapse id="nav-collapse" is-nav>
        <!-- Right aligned nav items -->
        <b-navbar-nav class="ml-auto">
          <b-navbar-nav right>
            <b-nav-item href="#" id="TextLayanan" text-black>Layanan</b-nav-item>
            <b-nav-item href="#" id="TextTim" text-black>Tim</b-nav-item>
            <b-nav-item href="#" id="TextTestimoni" text-black>Testimoni</b-nav-item>
            <b-nav-item href="#" id="TextHubungiKami" text-black>Hubungi Kami</b-nav-item>
          </b-navbar-nav>
        </b-navbar-nav>
      </b-collapse>
    </b-navbar>
    <b-navbar
      class="grey-1 pl-5 pr-5"
      toggleable="lg"
      variant="info"
      id="navbar"
      v-else
      v-on:scroll="handleScroll"
    >
      <b-navbar-brand href="#">
        <b-img
          :src="require('@/assets/images/logo-pesankan.png')"
          fluid
          alt="Responsive image"
          width="148"
          height="35"
          gravity="faces"
          crop="fill"
        ></b-img>
      </b-navbar-brand>

      <b-navbar-toggle target="nav-collapse"></b-navbar-toggle>

      <b-collapse id="nav-collapse" is-nav>
        <!-- Right aligned nav items -->
        <b-navbar-nav class="ml-auto">
          <b-navbar-nav right>
            <b-nav-item href="#" id="TextLayanan" text-black>Layanan</b-nav-item>
            <b-nav-item href="#" id="TextTim" text-black>Tim</b-nav-item>
            <b-nav-item href="#" id="TextTestimoni" text-black>Testimoni</b-nav-item>
            <b-nav-item href="#" id="TextHubungiKami" text-black>Hubungi Kami</b-nav-item>
          </b-navbar-nav>
        </b-navbar-nav>
      </b-collapse>
    </b-navbar>
  </div>
</template>

<script>
import $ from "jquery";

export default {
  data: function() {
    return {
      fixedTop: false
    };
  },
  methods: {
    handleScroll() {
      if ($(window).scrollTop() == 0) {
        this.fixedTop = false;
      } else if ($(window).scrollTop() > 1) {
        this.fixedTop = true;
      }
    }
  },
  created() {
    window.addEventListener("scroll", this.handleScroll);
  },
  destroyed() {
    window.removeEventListener("scroll", this.handleScroll);
  }
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->

<style lang="scss">
.grey-1 {
  background-color: #f8f8f8 !important;
}

.text-black {
  color: #000 !important;
}
</style>
