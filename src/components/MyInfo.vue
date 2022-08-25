<template>
    <div class="container">
        <div v-for="(card, index) in cards" :key="index" class="card">
            <img :src="card.img">
            <span>{{card.text}}</span>
        </div>
    </div>
</template>

<script>
export default {
    name: 'MyInfo',
    data() {
        return {
            cards: [
                {
                    text: 'DIGITAL COMICS',
                    img: require('../assets/img/buy-comics-digital-comics.png')
                },
                {
                    text: 'DC MERCHANDISE',
                    img: require('../assets/img/buy-comics-merchandise.png')
                },
                {
                    text: 'SUBSCRIPTION',
                    img: require('../assets/img/buy-comics-subscriptions.png')
                },
                {
                    text: 'COMIC SHOP LOCATOR',
                    img: require('../assets/img/buy-comics-shop-locator.png')
                },
                {
                    text: 'DC POWER VISA',
                    img: require('../assets/img/buy-dc-power-visa.svg')
                }
            ]
        }
    }
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
            padding:20px;
            align-items: center;

            img {
                width:2rem;
            }
            span {
                color:white;
                font-size: 13px;
                margin-left: 5px;
                font-weight: 300;
            }
        }
    }
</style>