<template>
    <v-row justify="center"
      ><video width="70%" autoplay muted controls>
        <source src="~/assets/AURA video.mp4" type="video/mp4" /></video
    ></v-row>
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
