<template>
    <main>
        <div class="container">
            <Products/>
            <BestSellerProducts/>
        </div>
    </main>
</template>

<script>
import Products from '../sections/Products.vue';
import BestSellerProducts from '../sections/BestSellerProducts.vue';

export default {
    name: 'Main',
    components: {
        Products,
        BestSellerProducts
    }
}
</script>

<style lang="scss" scoped>
    main {
        background-image: url('../../assets/img/fondo-pag-speciali.jpg');
        margin-top: 40px;
    }
</style>