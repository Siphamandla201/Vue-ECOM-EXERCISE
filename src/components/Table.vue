<template>
    <div >
        <table>
            <thead>
                <tr>
                    <th>Edit</th>
                    <th>Name</th>
                    <th>Image</th>
                    <th>Price</th>
                    <th>Quantity</th>
                    <th>Opt</th>
                </tr>
            </thead>
            <tbody v-for=" Product in Product" :key="Product">
                <tr>
                    <td>
                        <button>Edit</button>
                    </td>
                    <td>{{Product.ProductName}}</td>
                    <td>{{Product.ProductImage}}</td>
                    <td>{{Product.ProductPrice}}</td>
                    <td>{{Product.ProductQuantity}}</td>
                    <td>
                        <button>+</button>
                        <button>-</button>
                    </td>
                </tr>
            </tbody>
        </table>
    </div>
</template>
<script>
export default {
    name: 'Table'
    
}
</script>
<style>
    
</style>