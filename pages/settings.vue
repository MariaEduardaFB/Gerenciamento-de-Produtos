<template>
    <v-container>
      <v-switch v-model="darkTheme" label="Tema Escuro"></v-switch>
    </v-container>
  </template>
  
  <script>
  export default {
    data() {
      return {
        darkTheme: false
      };
    },
    watch: {
      darkTheme(val) {
        this.$vuetify.theme.dark = val;
      }
    }
  }
  </script>
  