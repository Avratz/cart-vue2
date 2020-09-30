<template>
  <v-card class="mx-5 my-12" max-width="374">
    <v-img height="250" :src="productoData.imagen"></v-img>
    <v-card-title>{{ productoData.titulo }}</v-card-title>
    <v-card-text>$ {{ productoData.precio }}</v-card-text>
    <v-card-actions>
      <v-btn color="deep-purple lighten-2" text>Add To Cart</v-btn>
    </v-card-actions>
  </v-card>
</template>

<script>
export default {
  name: "Producto",
  props: {
    productoData: {
      type: Object,
      required: true,
    },
  },
};
</script>

<style lang="scss" scoped>
</style>