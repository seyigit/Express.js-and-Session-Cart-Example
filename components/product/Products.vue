


<template>
            <div class="product-container card shadow mr-5">
            <h3 class="text-center">Ürün Listesi</h3>
            <Product v-for="product in products" :key="product.id" :product="product"/>
            </div>
</template>

<script>
import Product from "./Product"
export default {
    components : {
        Product
    },
    props : {
        products : {
            type:Array,
            required : false,

        }
    }


}
</script>