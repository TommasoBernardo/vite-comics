<template>
    <footer>
        <div id="bg-footer">
            <section>
                <nav>
                    <h4>DC COMICS</h4>
                    <ul>
                        <li v-for="link, i in dcComicslinks " :key="i" >
                        <a :href="link.url" >{{link.text}}</a>
                        </li>
                    </ul>

                    <h4>SHOP</h4>
                    <ul>
                        <li v-for="link, y in shoplinks " :key="y" >
                            <a :href="link.url" >{{link.text}}</a>
                        </li>
                    </ul>
                    </nav>
                <nav>
                    <h4>DC</h4>
                    <ul>
                        <li v-for="link, x in dclinks " :key="x" >
                            <a :href="link.url" >{{link.text}}</a>
                        </li>
                    </ul>
                </nav>
                <nav>
                    <h4>SITES</h4>
                    <ul>
                        <li v-for="link, n in siteslinks " :key="n" >
                            <a :href="link.url" >{{link.text}}</a>
                        </li>
                    </ul>
                </nav>

            </section>

        </div>
       
        <div id="footer-bottom">
            <section>
                <button>SIGN-UP NOW!</button>
                
                <div>
                    <h4>FOLLOW US</h4>
               
                    <ul>
                        <li v-for="link, i in sociallinks" :key='i'>
                            <a href=""> <img :src="require(`../assets/img/${link.img}`)" :alt="link.text"></a>
                        </li>
                    </ul>

                </div>
            
            </section>
        </div>
        
    </footer>
    
</template>

<script>
export default {
  name: 'AppFooter',
  data(){
        return {
            dcComicslinks: [
                {
                    text: 'Charaters',
                    url: '#', 
                },
                {
                    text: 'Comics',
                    url: '#', 
                },
                {
                    text: 'Movies',
                    url: '#', 
                },
                {
                    text: 'TV',
                    url: '#', 
                },
                {
                    text: 'Games',
                    url: '#', 
                },
                {
                    text: 'Videos',
                    url: '#', 
                },
                {
                    text: 'News',
                    url: '#', 
                }
            ],
            shoplinks: [
                {
                    text:'Shop DC',
                    url: '#'
                },
                {
                    text:'Shop DC Collectibles',
                    url: '#'
                }
            ],
            dclinks: [
                {
                    text: 'Terms Of Use',
                    url: '#', 
                },
                {
                    text: 'Privacy policy (New)',
                    url: '#', 
                },
                {
                    text: 'Ad Choices',
                    url: '#', 
                },
                {
                    text: 'Advertising',
                    url: '#', 
                },
                {
                    text: 'Jobs',
                    url: '#', 
                },
                {
                    text: 'Subscription',
                    url: '#', 
                },
                {
                    text: 'Talent Workshops',
                    url: '#', 
                },
                  {
                    text: 'CPSC Certificates',
                    url: '#', 
                },
                  {
                    text: 'Ratings',
                    url: '#', 
                },
                  {
                    text: 'Shop Help',
                    url: '#', 
                },
                  {
                    text: 'Contact US',
                    url: '#', 
                }
            ],
            siteslinks: [
                {
                    text: 'DC',
                    url: '#', 
                },
                {
                    text: 'MAD Magazine',
                    url: '#', 
                },
                {
                    text: 'DC Kids',
                    url: '#', 
                },
                {
                    text: 'DC Universe',
                    url: '#', 
                },
                {
                    text: 'DC Power Visa',
                    url: '#', 
                }
               
            ],
            sociallinks: [
                {   
                    text:'facebook',
                    img: 'footer-facebook.png',
                    url: '#'
                     
                },
                {   
                    text:'twitter',
                    img: 'footer-twitter.png',
                    url: '#'
                     
                },
                {
                    text:'youtube',
                    img: 'footer-youtube.png',
                    url: '#'
                     
                },
                {
                    text:'pinterest',
                    img: 'footer-pinterest.png',
                    url: '#'
                     
                },
                {
                    text:'periscope',
                    img: 'footer-periscope.png',
                    url: '#'
                     
                }
            ],
        }
    }
}
</script>

<style scoped lang="scss">
footer {
    
    #bg-footer {
        background-image: url("../assets/img/footer-bg.jpg");
        width: 100%;
    
        section {
            background-image: url("../assets/img/dc-logo-bg.png");
            background-repeat: no-repeat;
            background-position: right;
            background-size: 45%;
            width: 75%;
            padding: 20px 0;
            margin: 0px auto;
            display: flex;
            h4 {
                color: white;
                margin: 15px 20px;
            }
            ul {
                margin: 0 20px;
                li{
                    list-style: none;
                    a {
                        text-decoration: none;
                        text-align: start;
                        color:#898989 ;
                        font-size: 12px;
                    }
                }
            }
        }
    }
    #footer-bottom {
        background-color:#303030 ;
        height: 100px;
        display: flex;
        align-items: center;
        
        section {
            width: 75%;
            margin: 0 auto;
            display: flex;
            justify-content: space-between;
            align-items: center;
            button {
                border: 1px solid #0282f9 ;
                color: white;
                background-color: #303030 ;
                padding: 12px;
                font-size: 18px;
                font-weight: bold;
                cursor: pointer;
                
                &:hover {
                    background-color:#0282f9 ;
                }
            }
            div {
                display: flex;
                align-items: center;
                h4 {
                    color: #0281f7;
                    margin-right: 18px;
                }
                
                li {
                    margin: 0 6px;
                    display: inline-block;
                    img {
                        width: 30px;
                    }
                }
            }
           
        }
    }
    
}
</style>