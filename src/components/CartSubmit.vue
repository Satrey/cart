<template>
  <div>
    <v-container>
      <v-card class="ma-2 pa-4 align-center" elevation="10">
        <div class="d-flex">
          <v-card-title class="mt-0"
            >Товаров : 2 
          </v-card-title>
          <v-spacer></v-spacer>
          <v-btn color="red"><v-icon>mdi-cart-off</v-icon></v-btn>
        </div>
        <hr />
        <v-btn class="mt-4" color="green" width="100%"><h2>19.99$</h2></v-btn>
      </v-card>
    </v-container>
  </div>
</template>
<script>
export default {
  name: "CartProductCard",
};
</script>

<style lang="scss" scoped>
.price {
  color: rgb(0, 124, 6);
}
</style>