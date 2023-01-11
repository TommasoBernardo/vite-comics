
<script>
import ListComponent from './ListComponent.vue'
export default {
    name: 'AppMain',
    components:{
        ListComponent
            },
            data(){
            return{
                comicsList: [
                {
                    "thumb": "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2018/09/AC1000_DLX_162-001_HD_5ba13723281ab0.37845353.jpg?itok=ZsI-C5eX",
                    "price": "$19.99",
                    "series": "Action Comics",
                    "type": "comic book"
                },
                {
                    "thumb": "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2020/09/AV1976_01_300-001_HD_5f738f6e39ddd7.18205602.jpg?itok=VgdYdJ01",
                    "price": "$3.99",
                    "series": "American Vampire 1976",
                    "type": "comic book"
                },
                {
                    "thumb": "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/gn-covers/2018/08/AQMv4_UW_153-001_HD_5b7efa1745a9b8.08589135.jpg?itok=HPTtnrsb",
                    "price": "$16.99",
                    "series": "Aquaman",
                    "type": "graphic novel"
                },
                {
                    "thumb": "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2018/06/batgirl_v5_1_5b23e1f1124941.50950783.jpg?itok=VnrJah76",
                    "price": "$2.99",
                    "series": "Batgirl",
                    "type": "comic book"
                },
                {
                    "thumb": "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2018/09/BM_56_300-001_HD_5ba137a85c3bf3.33122291.jpg?itok=3FHJQYJZ",
                    "price": "$3.99",
                    "series": "Batman",
                    "type": "comic book"
                },
                {
                    "thumb": "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2018/09/BM_56_300-001_HD_5ba137a85c3bf3.33122291.jpg?itok=3FHJQYJZ",
                    "price": "$2.99",
                    "series": "Batman Beyond",
                    "type": "comic book"
                },
                {
                    "thumb": "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2019/08/BMSM_5d4361b7116261.74371456.jpg?itok=kEDR2OL8",
                    "price": "$3.99",
                    "series": "Batman/Superman",
                    "type": "comic book"
                },
                {
                    "thumb": "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2020/09/BMSMANN_01_300-001_HD_5f5ff17fa1d665.74704970.jpg?itok=azz5sfGk",
                    "price": "$4.99",
                    "series": "Batman/Superman Annual",
                    "type": "comic book"
                },
                {
                    "thumb": "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2020/09/BMTJWZ_01_300-001_HD_5f5ff2307dcb37.34652945.jpg?itok=VswVjLR8",
                    "price": "$5.99",
                    "series": "Batman: The Joker War Zone",
                    "type": "comic book"
                },
                {
                    "thumb": "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2020/08/cover-v2_5f40314645a734.37285065.png?itok=ImNM2QBY",
                    "price": "$6.99",
                    "series": "Batman: Three Jokers",
                    "type": "comic book"
                },
                {
                    "thumb": "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2020/10/BMWK_HQ_01_300-001_HD_5f7cb4945e13f6.89501032.jpg?itok=sVwALbUX",
                    "price": "$4.99",
                    "series": "Batman: White Knight Presents: Harley Quinn",
                    "type": "comic book"
                },
                {
                    "thumb": "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/gn-covers/2019/04/CTWv1_CC_144-001_HD_5ca5299a751963.53054221.jpg?itok=ooPaoLDq",
                    "price": "$16.99",
                    "series": "Catwoman",
                    "type": "graphic novel"
                }
            ],
            }
        }
    }

</script>

<template>
    <main>
        <section id="card">
            <div>
                <div class="jumbotron">
        </div>
 <section class="list-component">
            <div class="wrapper">
                <h4 class="title"> CURRENT SERIES </h4>
                <div class="cards">
                    <ListComponent v-for="item in comicsList" :path="item.thumb" :price="item.price"
                        :series="item.series" :type="item.type" />
                </div>
                <a href="#"> LOAD MORE </a>
            </div>
        </section>
            </div>
        </section>
        <section id="images">
            <div class="images-flex">
                <div>
                <img class="img-1" src="../assets/img/buy-dc-power-visa.svg" alt="visa">
                <span>DC POWER VISA</span>
            </div>
            <div>
                <img src="../assets/img/buy-comics-digital-comics.png" alt="digital">
                <span>DIGITAL COMICS</span>
            </div>
            <div>
                <img src="../assets/img/buy-comics-merchandise.png" alt="merch">
                <span>DC MERCHANDISE</span>
            </div>
            <div>
                <img src="../assets/img/buy-comics-subscriptions.png" alt="sub">
                <span>SUBSCRIPTION</span>
            </div>
            <div>
                <img src="../assets/img/buy-comics-shop-locator.png" alt="shoplocator">
                <span>COMIC SHOP LOCATOR</span>
            </div>
            </div>
        </section>
    </main>
</template>



<style lang="scss" scoped>
#dc-images>div,
#products>div{
    margin: 0 auto;
    width: 80%;
}
#card{
    background-color: #1c1c1c;
    color: white;
    
}
#images{
    background-color: rgb(49, 126, 235);
    display: flex;
    align-content: center;
    justify-content: space-around;
    padding: 50px 0;
    div{
        display: flex;
        gap: 10px;
        align-items: center;
        color: white;
        font-weight: bold;
    }
    img{
    height: 50px;
    }
    .img-1{
        width: 45px;
    }
    .images-flex{
        display: flex;
        justify-content: space-around;
        align-content: center;
    }
}

.jumbotron {
    background-image: url(../assets/img/jumbotron.jpg);
    background-size: cover;
    background-repeat: no-repeat;
    height: 500px;
}
.list-component {
    position: relative;
    padding-top: 4rem;
    h4.title {
        color: white;
        background-color: #0282f9;
        width: fit-content;
        font-size: 2rem;
        padding: .4rem .8rem;
        position: absolute;
        top: -20px;
    }
    .cards {
        display: flex;
        justify-content: center;
        flex-wrap: wrap;
    }
    a {
        display: block;
        width: fit-content;
        text-decoration: none;
        color: white;
        background-color:  #0282f9;
        margin: 0 auto;
        padding: .5rem 2.5rem;
        font-size: 1.5rem;
        font-weight: bold;
        margin-bottom: 1rem;
    }
}

</style>