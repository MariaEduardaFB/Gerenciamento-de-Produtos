<template>
    <v-container>
      <v-text-field label="Buscar Produto" v-model="searchTerm"></v-text-field>
      <v-btn @click="searchProduct">Buscar</v-btn>
      <v-form v-if="product">
        <v-text-field label="Nome do Produto" v-model="product.name"></v-text-field>
        <v-text-field label="Descrição" v-model="product.description"></v-text-field>
        <v-text-field label="Preço" v-model="product.price"></v-text-field>
        <v-btn @click="updateProduct">Atualizar</v-btn>
      </v-form>
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
      updateProduct() {
        // Código para atualizar o produto
      }
    }
  }
  </script>
  