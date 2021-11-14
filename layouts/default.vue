<template>
  <v-app>
    <v-main>
      <Nuxt />
    </v-main>
    <v-footer
      :absolute="!fixed"
      app
      class="justify-center justify-sm-space-between py-4"
    >
      <a href="https://www.instagram.com/hipmijaya/" target="_blank">
        HIPMI JAYA
        <v-icon>mdi-instagram</v-icon>
      </a>
      <span
        >&copy; {{ new Date().getFullYear() }} HIPMI Jaya x Manual Jakarta. All
        Rights Reserved.
      </span>
    </v-footer>
  </v-app>
</template>

<script>
export default {
  data() {
    return {
      clipped: false,
      drawer: false,
      fixed: false,
      items: [
        {
          icon: 'mdi-apps',
          title: 'Welcome',
          to: '/',
        },
        {
          icon: 'mdi-chart-bubble',
          title: 'Inspire',
          to: '/inspire',
        },
      ],
      miniVariant: false,
      right: true,
      rightDrawer: false,
      title: 'Vuetify.js',
    }
  },
}
</script>
