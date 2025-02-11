<template>
  <v-card
    max-width="374"
  >
    <template v-slot:loader="{ isActive }">
      <v-progress-linear
        :active="isActive"
        color="deep-purple"
        height="4"
        indeterminate
      ></v-progress-linear>
    </template>
    <v-img
      height="250"
      :src="''+props.item.src"
    ></v-img>

    <v-card-item>
      <v-card-title>{{ props.item.title }}</v-card-title>

    </v-card-item>

    <v-card-text>
      <div class="my-4 text-subtitle-1">
        {{ props.item.preco }}
      </div>

      <div>{{ props.item.descricao }}</div>
    </v-card-text>
    <v-card-actions>
      <v-btn
        color="deep-purple-lighten-2"
        text="Comprar"
        block
        border
      ></v-btn>
    </v-card-actions>
  </v-card>
</template>
<script setup>
const props = defineProps({ item: { required: false } });
</script>
