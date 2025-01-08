<template>
  <v-card
    ><v-card-title>{{ props.item }}</v-card-title
    ><v-card-text class="text-blue">Alguma descrição do produto</v-card-text
    ><v-card-actions><v-spacer/><v-btn color="green" variant="outlined" append-icon="mdi-cart-outline"></v-btn></v-card-actions></v-card
  >
</template>
<script setup>
const props = defineProps({ item: { required: false } });
</script>
