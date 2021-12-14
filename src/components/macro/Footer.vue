<template>
    <footer>
        <div class="container">
            <Logo alt-text="Logo Footer con salsa piccante" />
            Lorem ipsum dolor sit amet consectetur adipisicing elit. Molestiae esse sed laudantium quasi quidem fugit optio consectetur labore dicta natus. Sed error rerum qui recusandae perferendis. Quo amet voluptatem recusandae!
        </div>
    </footer>
</template>

<script>
import Logo from '../commons/Logo.vue';

export default {
    name: 'Footer',
    components: {
        Logo
    }
}
</script>

<style lang="scss" scoped>
    footer {
        padding: 40px 0;
        background-image: url('../../assets/img/footer-montagne-bottom.jpg');
        background-repeat: no-repeat;
        background-position: bottom;
    }
</style>