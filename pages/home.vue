<template>
    <v-container>
      <v-row>
        <v-col>
          <v-btn style="background-color: teal; color: white;" @click="navigateTo('add')">Cadastrar Produto</v-btn>
          <v-btn @click="navigateTo('view')">Visualizar Produto</v-btn>
          <v-btn @click="navigateTo('edit')">Editar Produto</v-btn>
          <v-btn @click="navigateTo('delete')">Deletar Produto</v-btn>
        </v-col>
      </v-row>
    </v-container>
  </template>
  
  <script>
  export default {
    methods: {
      navigateTo(route) {
        this.$router.push({ name: route });
      }
    }
  }
  </script>
  