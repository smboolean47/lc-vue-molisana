<template>
   <div class="product">
        <img :src="product.src" :alt="product.titolo">
        <h3>{{product.titolo}}</h3>
    </div>
</template>

<script>
export default {
    name: 'CardProduct',
    props: {
        product: Object
    }
}
</script>

<style lang="scss" scoped>
    .product {
        background-color: #fff;
        // width: calc(25% - 10px);
        // margin: 5px;
        padding: 20px 15px;

        img {
            width: 100%;
        }

        h3 {
            text-align: center;
        }
    }
</style>