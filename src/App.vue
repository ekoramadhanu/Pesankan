<template>
  <div id="app" class>
    <!-- Navbar  -->
    <Navbar />
    <!-- End Navbar -->

    <!-- Jumbotron -->
    <div>
      <b-jumbotron class="grey-1 p-0 m-0 jumbotron-pesankan">
        <b-row>
          <b-col class="middle" lg="6" md="6" sm="12">
            <h1 class="roboto">Pesankan</h1>
            <h3>
              Sebuah Aplikasi yang memudahkan Ibu rumah tangga untuk berbelanja produk segar dan
              memasak berdasarkan konsumsi gizi keluarga.
            </h3>
            <br />
            <b-button pill class="mr-2 green border-green" variant="primary" href="#">Unduh Sekarang</b-button>
            <b-button
              id="btn-more"
              class="border-green text-green"
              pill
              variant="outline-success"
              href="#"
              @mouseover="btnOver"
            >pelajari Lebih Lanjut</b-button>
          </b-col>

          <b-col lg="6" md="6" sm="12" class="p-0">
            <b-img
              class="image-pesankan"
              :src="require('@/assets/images/jumbotron.png')"
              fluid
              alt="Responsive image"
              width="729"
              height="539"
              gravity="faces"
              crop="fill"
            ></b-img>
          </b-col>
        </b-row>
      </b-jumbotron>
    </div>
    <!-- End Jumbotron -->
    <h4 class="text-center mt-2 text-green">Layanan</h4>
    <hr class="line-green" />
    <!--  baris pertama -->
    <b-row class="mr-5 ml-5 mt-3 row-layanan">
      <b-col xl="4" lg="4" md="4" xs="12" class="cardLayanan">
        <Card
          images="24-hours-delivery"
          title="aktif selama 24/7"
          subtitle="Seluruh layanan kami  akan membantu selama 24 jam non stop sehingga belanja bisa kapapun tanpa perlu khawatir jika barang kehabisan"
        />
      </b-col>
      <b-col xl="4" lg="4" md="4" xs="12" class="cardLayanan">
        <Card
          images="shipped"
          title="opsi pengiriman"
          subtitle="Pengguna bisa menentukan tempat pengiriman belanja produk segar seperti telur, sayur, dan yang lain -lainnya.  "
        />
      </b-col>
      <b-col xl="4" lg="4" md="4" xs="12" class="cardLayanan">
        <Card
          images="preorder"
          title="pembelian bersifat preorder"
          subtitle="Pembelian di layanan kami ini bersifat pre order. dimana pengguna akan membeli terlebih dahulu , lalu barang akan sampai ketika tukang sayur belanja"
        />
      </b-col>
    </b-row>

    <!-- akhir  baris pertama -->
    <b-row class="mr-5 ml-5 mt-3 row-layanan">
      <b-col xl="4" lg="4" md="4" xs="12" class="cardLayanan">
        <Card
          images="24-hours-delivery"
          title="MELACAK BARANG BELANJAAN"
          subtitle="Pengguna bisa melakukan cek barang belanjaan sudah sampai dimana."
        />
      </b-col>
      <b-col xl="4" lg="4" md="4" xs="12" class="cardLayanan">
        <Card
          images="shipped"
          title="GARANSI PEMBELIAN"
          subtitle="Setelah produk segar telah sampai pengguna akan mendapatkan garansi selama kurang leebih 3 jam setelah barang diterima. "
        />
      </b-col>
      <b-col xl="4" lg="4" md="4" xs="12" class="cardLayanan">
        <Card
          images="preorder"
          title="PENGECEKAN GIZI "
          subtitle="Setiap minggu layanan kami akan memberikan pengecekan kepada pengguna untuk memberitahukan gizi "
        />
      </b-col>
    </b-row>
    <!-- akhir  baris kedua -->
    <div class="grey-1 mt-3 pt-3 pb-3">
      <h4 class="text-center text-green">Anggota Tim</h4>
      <hr class="line-green" />
      <b-row class="mr-5 ml-5">
        <b-col lg="6" md="6" sm="12">
          <Tim
            name="Muhammad Khaufillah"
            job="Perintis"
            overview="Some quick example text to build on the card and make up the bulk of the card's content."
          />
        </b-col>
        <b-col lg="6" md="6" sm="12">
          <Tim
            name="Eko Ramadhanu Aryputra"
            job="Perintis"
            overview="Some quick example text to build on the card and make up the bulk of the card's content."
          />
        </b-col>
      </b-row>
    </div>
    <!-- <h4 class="text-center mt-2">Testimoni</h4> -->
    <h4 class="text-center mt-2">Hubungi Kami</h4>
    <hr class="line-green" />
    <b-row class>
      <b-col lg="6" md="6" sm="12">
        <b-form class="mr-5 ml-5">
          <b-input
            id="inline-form-input-name inputName"
            class="mb-2 mr-sm-2 mb-sm-0"
            placeholder="Nama"
            size="150"
          ></b-input>
          <b-input
            id="inline-form-input-name inputEmail"
            class="mb-2 mr-sm-2 mb-sm-0 mt-2"
            placeholder="Alamat Email"
            size="150"
          ></b-input>
          <b-form-textarea
            class="mt-2"
            id="textarea"
            placeholder="Tulis Pesan Anda"
            rows="3"
            max-rows="6"
          ></b-form-textarea>
          <b-button class="mt-2 green text-white border-green" pill variant="success">Kirim Pesan</b-button>
        </b-form>
      </b-col>
      <b-col lg="5" md="5" sm="12"></b-col>
    </b-row>
    <!-- akhir dari hubungi kami -->
    <div class="grey-1 mt-3">
      <b-row class="pt-3 pl-5 pr-5">
        <b-col lg="3">
          <b-img
            :src="require('@/assets/images/logo-pesankan.png')"
            fluid
            alt="Responsive image"
            width="148"
            height="35"
          ></b-img>
          <p>Sebuah Aplikasi yang memudahkan aktivitas Ibu rumah tangga</p>
          <b-img
            class="mr-5"
            :src="require('@/assets/images/facebook-logo.svg')"
            fluid
            alt="Fluid image"
            width="15"
            height="15"
          ></b-img>
          <b-img
            class="mr-5"
            :src="require('@/assets/images/instagram (1).svg')"
            fluid
            alt="Fluid image"
            width="15"
            height="15"
          ></b-img>
          <b-img
            class="mr-5"
            :src="require('@/assets/images/linkedin (1).svg')"
            fluid
            alt="Fluid image"
            width="15"
            height="15"
          ></b-img>
        </b-col>
        <b-col lg="3">
          <p>Bantuan</p>
          <p>Kebijakan Privasi</p>
          <p>Syarat dan Ketentuan</p>
        </b-col>
        <b-col lg="3">
          <p>Kontak</p>
          <p>MT. Haryono Malang</p>
          <p>081234567890</p>
          <p>Pesankan@pesankan.com</p>
        </b-col>
        <b-col lg="3">
          <p>Unduh</p>
        </b-col>
      </b-row>
      <hr />
      <p class="text-center">copyright pesankan</p>
    </div>
    <!-- pembatas -->
  </div>
</template>

<script>
// import $ from "jquery";
import Card from "@/components/Card.vue";
import Tim from "@/components/Tim.vue";
// import Testimoni from "@/components/Testimoni.vue";
import Navbar from "@/components/Navbar.vue";

export default {
  components: {
    Card,
    Tim,
    Navbar
  }
};
</script>

<style lang="scss">
@font-face {
  font-family: "Roboto";
  src: url(./assets/fonts/Roboto-Regular.ttf);
}

.roboto {
  font-family: "Roboto";
}

.grey-1 {
  background-color: #f8f8f8 !important;
}

.green {
  background-color: #4abdac !important;
}

.border-green {
  border-color: #4abdac !important;
}
.text-green {
  color: #4abdac !important;
}
.m-0 {
  margin: 0px;
}

.p-0 {
  padding: 0px;
}

.middle {
  padding-top: 7rem !important;
  padding-left: 3rem !important;
}

.mr-2 {
  margin-right: 2rem;
}

.line-green {
  margin-top: -0.2rem !important;
  width: 5% !important;
  color: #4abdac !important;
  border: 0.8px solid #4abdac !important;
}

h1,
h2,
h3,
h4,
h5,
h6 {
  font-weight: normal !important;
}
.jumbotron-pesankan {
  overflow: hidden;
}

@media only screen and (min-width: 0px) and (max-width: 766px) {
  .cardLayanan {
    margin-top: 1rem;
  }
  .row-layanan {
    margin-top: 0px !important;
  }
  .image-pesankan {
    display: none;
  }
  .middle {
    padding-bottom: 7rem;
  }
}
</style>
