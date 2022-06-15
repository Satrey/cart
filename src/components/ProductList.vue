<template>
    <div>
       <h2 class="ms-6">Список товаров</h2>
       <ProductCard /> 
    </div>
</template>
<script>
import ProductCard from './ProductCard.vue'

export default {
    name: 'ProductList',

    components: {
        ProductCard,
    },

    data() {
        return {
            
        }
    },
}
</script>
<style lang="scss">
    
</style>