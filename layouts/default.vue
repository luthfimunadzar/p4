<template>
  <v-app>
    <v-main>
      <Nuxt />
    </v-main>
    <v-footer :absolute="!fixed" app class="justify-center py-4">
      <span
        >&copy; {{ new Date().getFullYear() }} HIPMI. All Rights Reserved.
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
