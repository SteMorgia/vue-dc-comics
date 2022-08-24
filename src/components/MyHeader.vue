<template>
    <header>
        <img src="../assets/img/dc-logo.png" alt="dc-logo">
        <nav>
            <ul>
                <li v-for="(link, index) in links" :key="index" >
                    <a :href="link.url" :class="link.active?'active':''" >{{link.text}}</a>
                </li>
            </ul>
        </nav>
    </header>
</template>

<script>
export default {
    name: 'MyHeader',
    data() {
        return {
            links: [
                {
                    text: 'CHARACTERS',
                    url: '#',
                    active: false
                },
                {
                    text: 'COMICS',
                    url: '#',
                    active: true
                },
                {
                    text: 'MOVIES',
                    url: '#',
                    active: false
                },
                {
                    text: 'TV',
                    url: '#',
                    active: false
                },
                {
                    text: 'GAMES',
                    url: '#',
                    active: false
                },
                {
                    text: 'COLLECTIBLES',
                    url: '#',
                    active: false
                },
                {
                    text: 'VIDEOS',
                    url: '#',
                    active: false
                },
                {
                    text: 'FANS',
                    url: '#',
                    active: false
                },
                {
                    text: 'NEWS',
                    url: '#',
                    active: false
                },
                {
                    text: 'SHOP',
                    url: '#',
                    active: false
                }
            ]
        }
    }
    }
</script>

<style scoped lang="scss">
    @import '../styles/vars.scss';

    header {
        text-align: center;
        display: flex;
        align-items: center;
        justify-content: space-around;
        margin:10px 0px;

        ul {
            list-style: none;
            margin: 30px;

            li {
                display:inline-block;
                margin: 0px 5px;

                a {
                    color: black;
                    text-decoration: none;
                    padding:10px;

                    &.active, &:hover {
                        background-color: $brand_color;
                    }
                }
            }
        }
    }
</style>