<template>
    <div class="cart-container card shadow">
        <h3 class="text-center ">Sepet</h3>
        <Alert v-if="cart.length == 0 || !cart"/>
        <Carditems v-else :cart="cart"/>
        <CartFooter />
    </div>
</template>
<script>
import Alert from "./Alert"
import CartFooter from "./CartFooter"
import Carditems from "./Cartitems"
export default {
    components : {  
        Alert,
        CartFooter,
        Carditems


    },
    props : {
        cart :{
            type : Array,
            required : false
        }
    }
}
</script>