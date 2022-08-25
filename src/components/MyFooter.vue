<template>
    <footer>
        <section class="upper-footer">
            <div class="container">
                <div class="container-left">
                    <div v-for="(link, index) in links" :key="index" class="footer-links">
                        <h4>{{link.title}}</h4>
                        <ul>
                            <li v-for="(innerLink,innerIndex) in link.links" :key="innerIndex">
                                <a href="#">{{innerLink}}</a>
                            </li>
                        </ul>
                    </div>
                </div>
                
                <div class="container-right">
                    <div class="footer-logo">
                        <img src="../assets/img/dc-logo-bg.png" alt="footer-logo">
                    </div>
                </div>
            </div>
            
        </section>
        <section class="lower-footer">
            <div>
                <button>SIGN-UP NOW</button>
            </div>
            <div>
                <span class="text">FOLLOW US</span>
            </div>
        </section>
    </footer>
</template>

<script>
export default {
    name: 'MyFooter',
    data() {
        return {
            links: [
                {
                    title: 'DC COMICS',
                    links: [
                        'Characters',
                        'Comics',
                        'Movies',
                        'TV',
                        'Games',
                        'Videos',
                        'News'
                    ]
                },
                {
                    title: 'DC',
                    links: [
                        'Tern Of Use',
                        'Privacy Policy(New)',
                        'Ad Choices',
                        'Advertising',
                        'Jobs',
                        'Subscriptions',
                        'Talent Workshops',
                        'CPSC Certificates',
                        'Ratings',
                        'Shop Help'
                    ] 
                },
                {
                    title: 'SITES',
                    links: [
                        'DC',
                        'MAD Magazine',
                        'DC Kids',
                        'DC Universe',
                        'DC Power Visa'
                    ] 
                },
                {
                    title: 'SHOP',
                    links: [
                        'Shop DC',
                        'Shop DC Collectibles'
                    ] 
                }
            ]
        }
    }
}
</script>

<style scoped lang="scss">
@import '../styles/vars.scss';
    .upper-footer {
        
        background-image: url(../assets/img/footer-bg.jpg);
        
        .container {
            display:flex;
            justify-content: space-around;
            width:100%;

            .container-left {
                display:flex;
                margin-top:15px;
            }
            
        }
        .footer-links {
            margin:10px 20px;
            ul {
                list-style: none;
                a {
                    color:grey;
                    text-decoration: none;
                }
            }
            h4 {
                color:white;
            }
        }
        .footer-logo img {
            width:300px;
            
        }
    }
    .lower-footer {
        display:flex;
        justify-content: space-around;
        align-items: center;
        background-color: #2B2B2B;
        padding:20px;
        button {
            padding:5px;
            background-color:#2B2B2B;
            border-color:$brand_color;
            color:white;
        }
        .text {
            color:$brand_color;
        }
    }
</style>