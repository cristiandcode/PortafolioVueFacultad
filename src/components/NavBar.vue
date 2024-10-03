<template>
    <v-app-bar app color="black" dark flat class="px-12" >
      <v-btn >
        <v-icon color="yellow" left class="mr-2">fas fa-signature</v-icon> Cristian Programmer
      </v-btn>
      
  
      <v-spacer></v-spacer>
      <v-btn text @click="scroll('home')" class="text-yellow">Inicio</v-btn>
      <v-btn text @click="scroll('about')"  >Acerda de mi</v-btn>
      <v-btn text @click="scroll('portfolio')"  >Portafolio</v-btn>
      <v-btn text @click="scroll('services')" > Servicios</v-btn>
      <v-btn text @click="scroll('page')"  > Pagina</v-btn>
      <v-btn text @click="scroll('biog')"  > Biografia</v-btn>
      <v-btn text @click="scroll('contact')"  > Contacto</v-btn>
    </v-app-bar>
  </template>
  
  <script>
  export default {
    methods: {
      scroll(refName) {
        const element = document.getElementById(refName);
        element.scrollIntoView({ behavior: "smooth" });
      },
    },
  };
  </script>
  
  <style>
  </style>