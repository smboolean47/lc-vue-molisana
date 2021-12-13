<template>
    <header>
        <div class="container">
            <div class="logo">
                <img src="../assets/img/la-molisana-logo.png" alt="Logo">
            </div>
            <nav>
                <ul>
                    <!-- <li><a href="#">Home</a></li>
                    <li><a class="active" href="#">Prodotti</a></li>
                    <li><a href="#">Chi Siamo</a></li>
                    <li><a href="#">Contatti</a></li> -->
                    <li v-for="(link, index) in links" :key="index"><a :class="{ active: link.current }" :href="link.url">{{link.text}}</a></li>
                </ul>
            </nav>
        </div>
    </header>
</template>

<script>
export default {
    name: 'Header',
    data() {
        return {
            // dati del componente
            links: [
                {
                    text: "Home",
                    url: "#",
                    current: false,
                },
                {
                    text: "Prodotti",
                    url: "#",
                    current: true,
                },
                {
                    text: "Chi Siamo",
                    url: "#",
                    current: false,
                },
                {
                    text: "Contatti",
                    url: "#",
                    current: false,
                },
            ]
        }
    }
}
</script>

<style lang="scss" scoped>
@import '../assets/style/partials/variables.scss';

    header {
        text-align: center;
    }

    nav {
        margin-top: 20px;
        // nav ul {}
        ul {
            display: flex;
            justify-content: center;
            list-style: none;

            // nav ul li
            li a {
                display: inline-block;
                padding: 15px 20px;
                text-decoration: none;
                color: #000;
                // nav ul li a.active, nav ul li a:hover
                &.active, &:hover {
                    background-color: $secondaryColor;
                }
            }
        }
    }

</style>