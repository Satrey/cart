<template>
    <div>
        <h2>Список покупок</h2>
        <CartListItem />
        <CartSubmit />
    </div>
</template>
<script>
import CartListItem from './CartListItem.vue'
import CartSubmit from './CartSubmit.vue'

export default {
    name: 'CartList',

    components: {
        CartListItem,
        CartSubmit,
    },

    data() {
        return {
            
        }
    },
}
</script>
<style lang="">
    
</style>