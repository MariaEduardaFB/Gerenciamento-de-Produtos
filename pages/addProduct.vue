<template>
    <v-container>
      <v-form>
        <v-text-field label="Nome do Produto" v-model="product.name"></v-text-field>
        <v-text-field label="Descrição" v-model="product.description"></v-text-field>
        <v-text-field label="Preço" v-model="product.price"></v-text-field>
        <v-btn @click="saveProduct">Salvar</v-btn>
      </v-form>
    </v-container>
  </template>
  
  <script>
  export default {
    data() {
      return {
        product: {
          name: '',
          description: '',
          price: ''
        }
      };
    },
    methods: {
      saveProduct() {
        // Código para salvar o produto
      }
    }
  }
  </script>
  