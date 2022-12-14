<template>
    <div>
        <div class="Product" v-for=" Product in Product"  :key="'Product'">
            <img :src="Product.ProductImage" :alt="Product.ProductName">
            <h5>{{Product.ProductName}}</h5>
            <h3>{{Product.ProductPrice}}</h3>
            <button @click="addButtons">Purchase</button>
        </div> 
    </div>
</template>
<script>
export default {
    name : 'Product',

    data () {
        return {
            Product : [
                {
                    ProductImage : "https://i.pinimg.com/236x/af/69/5e/af695e7f3c819bc784b4d0ebd19ce67f.jpg",
                    ProductName : "Stretch Cotton Flap Cap",
                    ProductPrice : "R250"
                }
            ]
        }
    },

    methods: {
        addButtons : function () {
            alert('item has been added to cart')
        }
    },

}
</script>
<style>
    
</style>