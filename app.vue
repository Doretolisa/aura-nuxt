<template>
  <v-app>
  <v-container fluid>
    <v-system-bar color="black" class="text-center" app>
      <v-row justify="center">PARCELE EM ATE 10X | CUPOM DE DESCONTO: BEAUTY253219</v-row>
    </v-system-bar>
    <v-app-bar color="deep-purple-lighten-1 py-3" >
      <v-row justify="center">
        <h1 class="logostyle pt-4">
          AURA
          <span style="font-family: 'Montserrat', sans-serif; font-size: 0.18em"
            >REALCE SUA BELEZA INTERIOR</span
          >
        </h1>
      </v-row>

      <v-spacer></v-spacer>

      <v-text-field
        class="mt-6 mr-4"
        :rounded="true"
        prepend-inner-icon="mdi-magnify"
        variant="outlined"
        placeholder="Buscar Produto"
      ></v-text-field>
    </v-app-bar>
    <v-main>
    <v-container>
      <v-row class="text-black"
        >
        <v-col v-for="item in menu" class="text-center"> <v-btn variant="text" :to="item.url">{{ item.text }}</v-btn></v-col>
      </v-row>
      <v-row><v-col cols="12"> <NuxtPage/></v-col></v-row>
      </v-container></v-main
    >
  </v-container></v-app>
</template>

<script setup>
const menu = [
  {
    text: "Todos os produtos",
    url: "/produtos",
  },
  {
    text: "Aura Summer",
    url: "/summer",
  },
  {
    text: "Maquiagem",
    url: "/maquiagem",
  },
  {
    text: "Lojas",
    url: "/lojas",
  },
];
</script>

<style>
.logostyle {
  font-family: "Hatton", sans-serif;
  color: white;
  font-size: 4rem;
}

@font-face {
  font-family: "Hatton";
  src: url("~/assets/Hatton-Medium.otf") format("opentype");
}

@font-face {
  font-family: "Montserrat";
  src: url("~/assets/Montserrat.ttf");
}
</style>
