<template>
    <v-container>
      <v-text-field label="Buscar Produto" v-model="searchTerm"></v-text-field>
      <v-btn @click="searchProduct">Buscar</v-btn>
      <v-card v-if="product">
        <v-card-title>{{ product.name }}</v-card-title>
        <v-card-text>{{ product.description }}</v-card-text>
        <v-card-text>{{ product.price }}</v-card-text>
      </v-card>
    </v-container>
  </template>
  
  <script>
  export default {
    data() {
      return {
        searchTerm: '',
        product: null
      };
    },
    methods: {
      searchProduct() {
        // Código para buscar o produto
      }
    }
  }
  </script>
  