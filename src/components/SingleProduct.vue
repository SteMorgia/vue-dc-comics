<template>
    <div class="product-card">
        <img :src="imageSrc"/>
        <h3>{{title}}</h3>
    </div> 
</template>

<script>
export default {
    name:'SingleProduct',
    props:{
        imageSrc: String,
        title: String
    }
}
</script>

<style scoped lang="scss">
    .product-card {
        flex-basis: 16%;
        img {
            max-width: 100%;
        }
        h3 {
            font-size: 16px;
        }
    }
</style>