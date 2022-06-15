<template>
  <div>
    <v-container>
      <v-card
        class="ma-2 pa-4 align-center"
        elevation="10"
        v-for="i in 5"
        :key="i"
      >
        <v-card-title class="mt-0"> The Fullstack hoodie </v-card-title>
        <hr />
        <div class="d-flex align-center">
          <v-card-text class="ma-0">
            This is a product card # {{ i }}
          </v-card-text>
          <v-card-subtitle class="ma-0">
            <h2 class="price">19.99$</h2>
          </v-card-subtitle>
          <v-spacer></v-spacer>
          <v-btn class="justify-end">В корзину</v-btn>
        </div>
      </v-card>
    </v-container>
  </div>
</template>
<script>
export default {
  name: "ProductCard",
};
</script>

<style lang="scss" scoped>
.price {
  color: rgb(0, 124, 6);
}
</style>