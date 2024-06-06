<template>
    <v-container>
      <v-text-field label="Buscar Produto" v-model="searchTerm"></v-text-field>
      <v-btn @click="searchProduct">Buscar</v-btn>
      <v-card v-if="product">
        <v-card-title>{{ product.name }}</v-card-title>
        <v-card-text>{{ product.description }}</v-card-text>
        <v-card-text>{{ product.price }}</v-card-text>
        <v-btn color="red" @click="deleteProduct">Excluir</v-btn>
        <v-btn @click="cancelDelete">Cancelar</v-btn>
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
      },
      deleteProduct() {
        // Código para deletar o produto
      },
      cancelDelete() {
        this.product = null;
        this.searchTerm = '';
      }
    }
  }
  </script>
  