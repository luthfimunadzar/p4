<template>
  <div>
    <div class="hero" style="background-image: url('/hero.jpg')">
      <img src="/logo.png" alt="" class="logo" />
      <div class="wrap">
        <!-- <h5>{{ new Date().getFullYear() }}</h5> -->
        <h2>Pengusaha Pejuang,<br />Pejuang Pengusaha</h2>
        <h6>
          A Lexicon of Entrepreneurial Stories<br />Curated by HIPMI Jaya x
          Manual Jakarta
        </h6>
      </div>
    </div>
    <div class="showcase d-none">
      <img src="/depan.png" alt="" />
    </div>
    <div class="narasumber">
      <v-container>
        <v-row>
          <v-col cols="12" class="text-center">
            <h4 class="title-sec">Forewords By</h4>
            <span class="underline"></span>
          </v-col>
        </v-row>
        <v-row class="justify-center">
          <v-col
            v-for="item in sekapurs"
            :key="item.id"
            md="3"
            sm="3"
            cols="6"
            class="item-narasumber text-center"
          >
            <div class="d-inline-block circle">
              <v-avatar size="120">
                <img :src="item.img" />
              </v-avatar>
            </div>
            <h5>{{ item.nama }}</h5>
            <h6>{{ item.title }}</h6>
          </v-col>
        </v-row>
      </v-container>
    </div>
    <div class="narasumber gray">
      <v-container>
        <v-row>
          <v-col cols="12" class="text-center">
            <h4 class="title-sec">Inspiring Stories by</h4>
            <span class="underline"></span>
          </v-col>
        </v-row>
        <v-row class="justify-center">
          <v-col
            v-for="item in narasumbers"
            :key="item.id"
            md="3"
            sm="3"
            cols="6"
            class="item-narasumber text-center"
          >
            <div class="d-inline-block circle">
              <v-avatar size="120">
                <img :src="item.img" />
              </v-avatar>
            </div>
            <h5>{{ item.nama }}</h5>
            <h6>{{ item.title }}</h6>
          </v-col>
        </v-row>
      </v-container>
    </div>
    <div class="tujuan d-none">
      <v-container>
        <v-row>
          <v-col cols="12" class="text-center">
            <h4 class="title-sec">Tujuan dan Manfaat</h4>
            <span class="underline"></span>
          </v-col>
        </v-row>
        <v-row class="justify-center">
          <v-col cols="12" md="4" class="">
            <v-card class="py-8 px-6">
              <p>
                Pembuatan buku HIPMI Jaya yang timeless, kreatif, menggugah,
                relevan,mudah dibaca dan bermanfaat bagi banyak orang
              </p>
            </v-card>
          </v-col>
          <v-col cols="12" md="4" class="">
            <v-card class="py-8 px-6">
              <p>
                Publikasi kepada masyarakat umum dalam hal kontribusi anggota
                HIPMI Jaya yang substansial dalam dunia kewirausahaan di
                Indonesia
              </p>
            </v-card>
          </v-col>
          <v-col cols="12" md="4" class="">
            <v-card class="py-8 px-6">
              <p>
                Menjadi panduan atau acuan utama untuk kalangan kewirausahaan
                Jakarta khususnya anggota HIPMI Jaya, dalam pembentukan ide,
                pemecahan masalah, pada suatu usaha dalam industri tertentu
              </p>
            </v-card>
          </v-col>
        </v-row>
      </v-container>
    </div>
    <div class="latar">
      <v-container>
        <v-row class="align-center">
          <v-col cols="12" sm="3" md="4" class="text-left">
            <h4 class="title-sec text-left">Latar Belakang</h4>
            <span class="underline mb-0"></span>
          </v-col>
        </v-row>
        <v-row class="justify-center">
          <v-col cols="12" sm="4" md="4">
            <v-card class="py-8 px-6" elevation="0">
              <div class="text-center">
                <img src="/tools.png" alt="" class="mb-3" />
              </div>
              <p>
                Young entrepreneurs in the early stage and even the mature
                stage, need a <b>starter kit</b>, <b>guides</b> and
                <b>tools</b> that strengthen them to continue growing
              </p>
            </v-card>
          </v-col>
          <v-col cols="12" sm="4" md="4">
            <v-card class="py-8 px-6" elevation="0">
              <div class="text-center">
                <img src="/smart-city.png" alt="" class="mb-3" />
              </div>
              <p>
                Young entrepreneurs need to acknowledge how to transform into
                entrepreneurs whose <b>innovations</b> and work
                <b>make a lasting impact</b>.
              </p>
            </v-card>
          </v-col>
          <v-col cols="12" sm="4" md="4">
            <v-card class="py-8 px-6" elevation="0">
              <div class="text-center">
                <img src="/diversification.png" alt="" class="mb-3" />
              </div>
              <p>
                Young entrepreneurs need to know
                <b>how to manage the crisis</b>, and
                <b>hear perspectives</b> from other fellow young entrepreneurs,
                so that they have the confidence to remain as an
                <b>intact, efficient, problem-solving entrepreneurs. </b>
              </p>
            </v-card>
          </v-col>
          <v-col cols="12" sm="4" md="4">
            <v-card class="py-8 px-6" elevation="0">
              <div class="text-center">
                <img src="/architect.png" alt="" class="mb-3" />
              </div>
              <p>
                Young entrepreneurs need to
                <b
                  >understand fully the riddle, the ups and downs, the hi and
                  low</b
                >
                on how to build a business; a way to continue to
                <b>strengthen their perserverance</b> in building a business.
              </p>
            </v-card>
          </v-col>
          <v-col cols="12" sm="4" md="4">
            <v-card class="py-8 px-6" elevation="0">
              <div class="text-center">
                <img src="/cycle.png" alt="" class="mb-3" />
              </div>
              <p>
                Young entrepreneurs who owned and running the series of
                generation of <b>family businesses</b>, need to understand how
                to continue the business to survive, sustain, and grow even
                further.
              </p>
            </v-card>
          </v-col>
        </v-row>
      </v-container>
    </div>
    <div class="buku d-none">
      <v-container>
        <v-row class="align-center">
          <v-col cols="12" sm="6" md="8">
            <span class="underline"></span>
            <h6>Judul Buku</h6>
            <h3>Pengusaha Pejuang, Pejuang Pengusaha</h3>
            <h6>Tema</h6>
            <p>
              “ Tips Praktis untuk Pengusaha Baru dalam Memasuki Industri dengan
              Efektif ”
            </p>
          </v-col>
          <v-col cols="12" sm="6" md="4">
            <v-card elevation="0" color="py-10 px-8">
              <h6>Penulis</h6>
              <h4 class="mb-5">Member HIPMI Jaya</h4>

              <h6>Pelaksanaan</h6>
              <h5>Dibuat mulai</h5>
              <h4 class="mb-3">Oktober 2021 – Februari 2022</h4>
              <h5>Soft Launching</h5>
              <h4>16 Desember 2021</h4>
            </v-card>
          </v-col>
        </v-row>
      </v-container>
    </div>
    <div class="collab">
      <v-container>
        <v-row>
          <v-col class="text-center">
            <h4 class="title-sec pr-8">Collaboration Partners</h4>
            <span class="underline mr-8"></span>
          </v-col>
          <v-col cols="12" class="text-center">
            <img src="partner.png" alt="" class="mr-4" />
            <img src="partner2.png" alt="" class="mr-4" />
            <img src="partner3.png" alt="" />
          </v-col>
        </v-row>
      </v-container>
    </div>
    <div class="contact">
      <v-container>
        <v-row class="align-center">
          <v-col cols="12" offset="0" sm="8" offset-sm="2" md="6" offset-md="3">
            <h5 class="title-form">Pre-order #BukuHIPMIJaya now:</h5>
            <validation-observer ref="observer">
              <form id="contactForm" @submit.prevent="submit">
                <validation-provider
                  v-slot="{ errors }"
                  name="Name"
                  rules="required"
                >
                  <v-text-field
                    v-model="form.name"
                    :error-messages="errors"
                    label="Name:"
                    name="name"
                    required
                  ></v-text-field>
                </validation-provider>
                <v-text-field
                  v-model="form.angkatan_hipmi"
                  label="Angkatan HIPMI Jaya:"
                  name="Angkatan HIPMI Jaya"
                  type="number"
                ></v-text-field>
                <validation-provider
                  v-slot="{ errors }"
                  name="Email"
                  rules="required|email"
                >
                  <v-text-field
                    v-model="form.email"
                    :error-messages="errors"
                    label="Email:"
                    name="email"
                    required
                  ></v-text-field>
                </validation-provider>
                <validation-provider
                  v-slot="{ errors }"
                  name="Phone Number"
                  rules="required"
                >
                  <v-text-field
                    v-model="form.phone"
                    :error-messages="errors"
                    label="Phone Number:"
                    name="Phone Number"
                    required
                  ></v-text-field>
                </validation-provider>
                <validation-provider
                  v-slot="{ errors }"
                  name="Quantity of Books"
                  rules="required"
                >
                  <v-text-field
                    v-model="form.jumlah_eksemplar"
                    :error-messages="errors"
                    label="Quantity of Books You'd Like to Order:"
                    name="jumlah_eksemplar"
                    type="Quantity of Books"
                    required
                  ></v-text-field>
                </validation-provider>
                <validation-provider
                  v-slot="{ errors }"
                  name="Message"
                  rules="required"
                >
                  <v-textarea
                    v-model="form.message"
                    :error-messages="errors"
                    label="Message:"
                    name="Message"
                    required
                    no-resize
                  ></v-textarea>
                </validation-provider>
                <v-btn
                  color="primary"
                  class="
                    btn btn-primary
                    d-inline-block
                    mt-5
                    text-capitalize
                    font-weight-medium
                    py-3
                    px-8
                  "
                  type="submit"
                  elevation="0"
                  :disabled="loading"
                >
                  <span>Send Form</span>
                </v-btn>
                <v-progress-circular
                  v-if="loading"
                  indeterminate
                  color="primary"
                  class="ml-2 mt-4"
                ></v-progress-circular>
              </form>
            </validation-observer>
          </v-col>
        </v-row>
      </v-container>
      <img src="/footer-bg.png" alt="" class="footer-bg" />
    </div>
  </div>
</template>

<script>
export default {
  data() {
    return {
      loading: false,
      form: {
        name: null,
        angkatan_hipmi: null,
        email: null,
        phone: null,
        jumlah_eksemplar: null,
        message: null,
      },
      narasumbers: [
        {
          id: 6,
          img: '/narasumber1.jpeg',
          nama: 'Rama Datau',
          title: 'Panasonic - Electronic/Retail/FnB',
        },
        {
          id: 1,
          img: '/narasumber2.jpeg',
          nama: 'Afifuddin Kalla',
          title: 'Bumi Mineral Sulawesi - Energy',
        },
        {
          id: 3,
          img: '/narasumber3.jpeg',
          nama: 'Diatche Harahap',
          title: 'Titik Temu - F&B Balesin.id Tech',
        },
        {
          id: 4,
          img: '/narasumber4.jpeg',
          nama: 'David Christian',
          title: 'Evoware - Social Enterprise / Sustainability',
        },
        {
          id: 5,
          img: '/narasumber5.jpeg',
          nama: 'Muhammad Aghnia Syahputra',
          title: 'LP3i Indonesia - Education',
        },
        {
          id: 2,
          img: '/narasumber6.jpeg',
          nama: 'Yudha Permana',
          title: 'Newman Pearsons - Property',
        },
        {
          id: 9,
          img: '/narasumber7.jpeg',
          nama: 'Dina Albens',
          title: 'Albens Cider - Winery',
        },
        {
          id: 10,
          img: '/narasumber8.jpeg',
          nama: 'Harizah Persiana',
          title: 'Sekolah Merdeka Cita - Social Entreprise / Education',
        },
        {
          id: 11,
          img: '/narasumber9.jpeg',
          nama: 'Shinta Melodi',
          title:
            'INTMO by YIG, Ltd.Co Interior & Furnitures / Trade Export Import',
        },
        {
          id: 12,
          img: '/narasumber10.jpeg',
          nama: 'Anindyo Suhardono',
          title: 'Satria Akasa Investama - Investment',
        },
        {
          id: 13,
          img: '/narasumber11.jpeg',
          nama: 'Bona Herbert Simanjorang',
          title: 'Juma Berlian Exim - Agriculture / Export & Import',
        },
        {
          id: 8,
          img: '/narasumber12.jpeg',
          nama: 'Arif Satria Kurniagung',
          title: 'Level Tujuh - Event',
        },
        {
          id: 7,
          img: '/narasumber13.jpeg',
          nama: 'Sayed Muhammad',
          title: 'USS Feed - Media',
        },
        {
          id: 14,
          img: '/narasumber14.jpeg',
          nama: 'Melissa Hamid',
          title: 'Abumas Group & Picknick Yuk Nona Manis - Industrial & Retail',
        },
      ],
      sekapurs: [
        {
          id: 1,
          img: '/sekapur1.jpg',
          nama: 'Sona Maesana',
          title: 'on "Pengusaha Muda Jakarta"',
        },
        {
          id: 2,
          img: '/sekapur2.jpeg',
          nama: 'Sandiaga Uno',
          title: 'on "Tourism in Indonesia"',
        },
        {
          id: 3,
          img: '/sekapur3.jpeg',
          nama: 'Bahlila Lahadalia',
          title: 'on "Ease of doing Business in Indonesia"',
        },
        {
          id: 4,
          img: '/sekapur4.jpeg',
          nama: 'Erick Thohir',
          title: 'on "How UMKM and BUMN Collaborate in Indonesia"',
        },
        {
          id: 5,
          img: '/sekapur5.jpeg',
          nama: 'M. Lutfi',
          title: 'on "How to Maximize Trade in Indonesia"',
        },
        {
          id: 6,
          img: '/sekapur6.jpeg',
          nama: 'Abdul Latief',
          title: 'on "Founding HIPMI"',
        },
        {
          id: 7,
          img: '/sekapur7.jpeg',
          nama: 'Mardani H. Maming',
          title: 'on "Pengusaha Muda Indonesia"',
        },
      ],
    }
  },
  head() {
    return {
      title: 'Pengusaha Pejuang, Pejuang Pengusaha',
      meta: [
        // hid is used as unique identifier. Do not use `vmid` for it as it will not work
        {
          hid: 'description',
          name: 'description',
          content:
            'A Lexicon of Entrepreneurial Stories Curated by HIPMI Jaya x Manual Jakarta',
        },
        {
          hid: 'og:title',
          name: 'og:title',
          content: 'Pengusaha Pejuang Pejuang Pengusaha',
        },
        {
          hid: 'keywords',
          name: 'keywords',
          content:
            'Pengusaha Pejuang Pejuang Pengusaha, pengusaha, pejuang, buku',
        },
        {
          hid: 'og:description',
          name: 'og:description',
          content:
            'A Lexicon of Entrepreneurial Stories Curated by HIPMI Jaya x Manual Jakarta',
        },
      ],
    }
  },
  mounted() {
    // this.loading = true
  },
  methods: {
    async submit() {
      this.loading = true
      const scriptURL =
        'https://script.google.com/macros/s/AKfycbyA6qqc0ZnuHWLa0q4Nc23gM3j2iYsBlTcHT5DH1DB8YtGiZ7O7dsriyQbRboRma6Jt/exec'
      const sendingData = new FormData()
      sendingData.append('name', this.form.name)
      sendingData.append('phone', this.form.phone)
      sendingData.append('email', this.form.email)
      sendingData.append('angkatan_hipmi', this.form.angkatan_hipmi)
      sendingData.append('jumlah_eksemplar', this.form.jumlah_eksemplar)
      sendingData.append('message', this.form.message)

      await fetch(scriptURL, { method: 'POST', body: sendingData })
        .then(
          () =>
            this.$swal.fire({
              type: 'success',
              title: 'Message Sent!',
              text: 'Thank you, we will contact you very soon.',
            }),
          this.reset()
        )
        .catch(() =>
          this.$swal.fire({
            type: 'error',
            title: 'Oops',
            text: 'Theres something error please try again later.',
          })
        )
      this.loading = false
    },
    reset() {
      this.form.name = null
      this.form.email = null
      this.form.angkatan_hipmi = null
      this.form.phone = null
      this.form.jumlah_eksemplar = null
      this.form.message = null
      this.$refs.observer.reset()
    },
  },
}
</script>
