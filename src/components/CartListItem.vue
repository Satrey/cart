<template>
  <div>
    <v-container>
      <v-card
        class="ma-2 pa-4 align-center"
        elevation="10"
        v-for="i in 2"
        :key="i"
      >
        <div class="d-flex">
          <v-card-title class="mt-0"> The Fullstack hoodie </v-card-title>
          <v-spacer></v-spacer>
          <v-card-subtitle class="ma-0">
            <h2 class="price">{{totalPrice}}$</h2>
          </v-card-subtitle>
        </div>
        <hr />
        <div class="d-flex align-center">
          <v-card-text class="ma-0">
            Количество в корзине: {{ count }}
          </v-card-text>
          <v-spacer></v-spacer>
          <v-btn class="me-1" icon="mdi-plus" @click="incriment"></v-btn>
          <v-btn icon="mdi-minus" @click="decriment"></v-btn>
        </div>
      </v-card>
    </v-container>
  </div>
</template>
<script>
export default {
  name: "CartListItem",

  data() {
      return {
          count: 0,
          price: 5.99,
      }
  },
  computed: {
      totalPrice(){
          return parseFloat(this.count * this.price).toFixed(2);
      },
  },

  methods: {
      incriment(){
          this.count ++;
      },
      decriment(){
          if(this.count > 0) this.count --;
      },
  },

};
</script>

<style lang="scss" scoped>
.price {
  color: rgb(0, 124, 6);
}
</style>