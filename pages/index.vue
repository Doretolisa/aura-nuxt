<template>
  <v-container fluid
    ><v-row
      ><v-col cols='3' v-for="item in items"><Produto :item="item" /></v-col></v-row
  ></v-container>
</template>
<script setup>
const items = ["Blush", "batom", "sabonete", "corretivo"];
</script>
