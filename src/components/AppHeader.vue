<script>
export default {
name: 'AppHeader',
}
</script>

<template>
    <header>
    <!-- logo -->
        <img src="../assets/img/dc-logo.png"/>
        <nav>
            <!--lista-->
        <ul>
            <li><a class="color-list" href="#">
                CHARACTERS
            </a></li>
            <li><a class="color-list-special active" href="#">
                COMICS    
            </a></li>
            <li><a class="color-list" href="#">
                MOVIES
            </a></li>
            <li><a class="color-list" href="#">
                TV
            </a></li>
            <li><a class="color-list" href="#">
                GAMES
            </a></li>
            <li><a class="color-list" href="#">
                COLLECTIBLES
            </a></li>
            <li><a class="color-list" href="#">
                VIDEOS
            </a></li>
            <li><a class="color-list" href="#">
                FANS
            </a></li>
            <li><a class="color-list" href="#">
                NEWS
            </a></li>
            <li><a class="color-list" href="#">
                SHOP
            </a></li>
        </ul>
    </nav>
    </header>
  </template>
  


<style scoped lang="scss">
header{
    display: flex;
    justify-content: space-between;
    align-items: center;
    padding: 20px;
    margin: 0 auto;
    width: 80%;
    ul{
        display: flex;
        gap: 15px;
    }
    .active{
        border-bottom: 5px solid #0282f9;
        
    }

    .color-list-special{
        color: #0282f9;
        text-decoration: none;
    }
}
</style>