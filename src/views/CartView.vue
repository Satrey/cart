<template>
    <div class="mt-3">
        <v-container>
            <v-card class="card ma-1">
                <h1 class="text-center">Корзина с покупками</h1>
            </v-card>
        </v-container>    
        <v-container class="d-flex align-start justify-center">
            <v-card class="col-md-12 ma-1 pa-4 card text-center" width="30%" min-height="900">
                <CartList />
            </v-card>
            <v-card class="col-md-12 ma-1 pa-4 card" width="70%" min-height="900">
                <ProductList />
            </v-card>
        </v-container>
    </div>
</template>
<script>
import CartList from '../components/CartList.vue'
import ProductList from '../components/ProductList.vue'

export default {
    name: 'CartView',

    components: {
        CartList,
        ProductList,
    },
}
</script>
<style lang="scss">
// h1 {
//     text-shadow: 2px 2px 20px rgba(128, 128, 128, 0.582);
// }

.card {
    background-color: rgba(0, 133, 66, 0.781);
    text-shadow: 1px 1px 5px rgba(0, 0, 0, 0.582);
    color: aliceblue;
    border: 4px solid rgb(255, 255, 255);
    box-shadow: 4px 4px 14px rgba(78, 78, 78, 0.514);
}
</style>