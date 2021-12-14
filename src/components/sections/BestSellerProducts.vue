<template>
    <section>
        <h2>I prodotti più venduti</h2>
        
        <div class="products-list">
            <!-- <div class="product" v-for="(product, index) in products" :key="index">
                <img :src="product.src" :alt="product.titolo">
                <h3>{{product.titolo}}</h3>
            </div> -->
            <CardProduct v-for="(product, index) in products" :key="index" :product="product"/>
        </div>
    </section>
</template>

<script>
import CardProduct from '../commons/CardProduct.vue';
import products from '../../data/bestSeller.js';

export default {
    name: 'BestSellerProducts',
    components: {
        CardProduct
    },
    data() {
        return {
            products : products
        }
    }
}
</script>

<style lang="scss" scoped>

    section {
        border: 10px dotted red;
    }

    h2 {
        text-align: center;
        margin: 20px 0;
    }

    .products-list {
        display: flex;
        flex-wrap: wrap;
        
        > * {
            width: calc(50% - 10px);
            margin: 5px;
        }
    }
</style>