<template>
    <footer>
        <section class="upper-footer">
            <div class="footer-links">
                <h4>DC COMICS</h4>
                <ul>
                    <li>
                        <a href="#">Characters</a>
                    </li>
                    <li>
                        <a href="#">Comics</a>
                    </li>
                    <li>
                        <a href="#">Movies</a>
                    </li>
                    <li>
                        <a href="#">TV</a>
                    </li>
                    <li>
                        <a href="#">Games</a>
                    </li>
                    <li>
                        <a href="#">Videos</a>
                    </li>
                    <li>
                        <a href="#">News</a>
                    </li>
                </ul>
            </div>
            
            <div class="footer-links">
                <h4>DC</h4>
                <ul>
                    <li>
                        <a href="#">Characters</a>
                    </li>
                    <li>
                        <a href="#">Comics</a>
                    </li>
                    <li>
                        <a href="#">Movies</a>
                    </li>
                    <li>
                        <a href="#">TV</a>
                    </li>
                    <li>
                        <a href="#">Games</a>
                    </li>
                    <li>
                        <a href="#">Videos</a>
                    </li>
                    <li>
                        <a href="#">News</a>
                    </li>
                </ul>
            </div>

            <div class="footer-links">
                <h4>SITES</h4>
                <ul>
                    <li>
                        <a href="#">Characters</a>
                    </li>
                    <li>
                        <a href="#">Comics</a>
                    </li>
                    <li>
                        <a href="#">Movies</a>
                    </li>
                    <li>
                        <a href="#">TV</a>
                    </li>
                    <li>
                        <a href="#">Games</a>
                    </li>
                    <li>
                        <a href="#">Videos</a>
                    </li>
                    <li>
                        <a href="#">News</a>
                    </li>
                </ul>
            </div>

            <div class="footer-links">
                <h4>SHOP</h4>
                <ul>
                    <li>
                        <a href="#">Characters</a>
                    </li>
                    <li>
                        <a href="#">Comics</a>
                    </li>
                    <li>
                        <a href="#">Movies</a>
                    </li>
                    <li>
                        <a href="#">TV</a>
                    </li>
                    <li>
                        <a href="#">Games</a>
                    </li>
                    <li>
                        <a href="#">Videos</a>
                    </li>
                    <li>
                        <a href="#">News</a>
                    </li>
                </ul>
            </div>
            <div class="footer-logo">
                <img src="../assets/img/dc-logo-bg.png" alt="footer-logo">
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
    name: 'MyFooter'
}
</script>

<style scoped lang="scss">
@import '../styles/vars.scss';
    .upper-footer {
        display: flex;
        background-image: url(../assets/img/footer-bg.jpg);
        padding:30px;
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