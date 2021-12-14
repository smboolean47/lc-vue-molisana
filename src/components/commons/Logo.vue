<template>
    <div class="logo">
        <img :src="require(`../../assets/img/${logoFilename}`)" :alt="altText">
    </div>
</template>

<script>
export default {
    name: 'Logo',
    props: {
        altText: String
    },
    data() {
        return {
            logoFilename: "la-molisana-logo.png"
        }
    }
}
</script>

<style>

</style>