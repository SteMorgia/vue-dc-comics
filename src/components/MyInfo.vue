<template>
    <div class="container">
        <div class="card">
            <img src="../assets/img/buy-comics-digital-comics.png">
            <span>Bla Bla Bla</span>
        </div>
    </div>
</template>

<script>
export default {
    name: 'MyInfo'
}
</script>
    
<style scoped lang="scss">
@import '../styles/vars.scss';
    .container {
        display:flex;
        justify-content: center;
        align-items: center;
        background-color: $brand_color;

        .card {
            display:flex;
            flex-basis: 20%;
            padding:20px;
            align-items: center;

            img {
                width:3rem;
            }
            span {
                color:white;
                font-size: 15px;
                margin-left: 5px;
                font-weight: 300;
            }
        }
    }
</style>