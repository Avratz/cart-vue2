<template>
  <v-main>
    <v-row no-gutters>
      <v-col v-for="product in productos" :key="product.id" cols="12" sm="4">
        <producto :productoData="product" />
      </v-col>
    </v-row>
  </v-main>
</template>

<script>
import productosData from "../productos.json";
import Producto from "./Producto";
export default {
  name: "Main",
  components: { Producto },
  data() {
    return {
      productos: productosData,
    };
  },
};
</script>

<style lang="scss" scoped>
</style>