<template>
  <v-app :theme="theme">
    <v-fab location="top end" :icon="icon" @click="toggleTheme" icon-color="red" absolute app appear></v-fab>
    <v-main>
      <Resume />
    </v-main>
  </v-app>
</template>

<script>
export default {
  data() {
    return {
      theme: 'dark',
      icon: 'mdi-white-balance-sunny',
    }
  },
  methods: {
    toggleTheme() {
      this.theme = this.theme === 'light' ? 'dark' : 'light';
      this.icon = this.theme === 'light' ? 'mdi-weather-night' : 'mdi-white-balance-sunny'
    }
  }
}
</script>
