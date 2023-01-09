<template>
    <header>
        <img src="../assets/img/dc-logo.png" alt="logo dc comics">
        <ul>
            <li v-for="link, i in links" :key='i'>
                <a :href="link.url" :class="link.isActive ? 'active' : '' ">{{link.text}}</a>

            </li>
        </ul>
    </header>
</template>

<script>
export default {
    name: 'AppHeader',
    data() {
        return {
            links: [
                {
                    text: 'CHARACTERS',
                    url: '#',
                    isActive: false
                },
                {
                    text: 'COMICS',
                    url: '#',
                    isActive: true
                },
                {
                    text: 'MOVIES',
                    url: '#',
                    isActive: false
                },
                {
                    text: 'TV',
                    url: '#',
                    isActive: false
                },
                {
                    text: 'GAMES',
                    url: '#',
                    isActive: false
                },
                {
                    text: 'COLLECTIBLES',
                    url: '#',
                    isActive: false
                },
                {
                    text: 'VIDEOS',
                    url: '#',
                    isActive: false
                },
                {
                    text: 'FANS',
                    url: '#',
                    isActive: false
                },
                {
                    text: 'NEWS',
                    url: '#',
                    isActive: false
                },
                {
                    text: 'SHOP',
                    url: '#',
                    isActive: false
                }
            ]
        }
    }
}
</script>

<style scoped lang="scss">
    header {
        width: 75%;
        margin: 0px auto;
        display: flex;
        justify-content: space-between;
        align-items: center;
        height: 100px;
        
        img {
            width: 6%;
        }
        
        li {
            display:inline-block;
            margin: 0 8px;
            a {
                text-decoration: none;
                color: #494b68;
                font-size: 12px;
                font-weight: bold;
                padding-bottom: 40px ;
                transition-duration: 0.2s;
                
                &.active {
                    color: #0282f9 ;
                    border-bottom: 3px solid #0282f9;
                    padding-bottom: 38px;
                }
                &:hover {
                    color: #0282f9 ;
                    border-bottom: 3px solid #0282f9;
                    padding-bottom: 38px;
                    
                }
            }
        }
    }
</style>
Footer
© 2023 GitHub, Inc.