<template>
  <div class="container">
      <div class="center">
          <ul>
                <li v-for="element in itemsList" :key="element">
                    <img :src="element.img" :alt="element.text">
                    <a href="">{{ element.text }}</a>
                </li>
          </ul>
      </div>
  </div>
</template>

<script>
import item1 from '../assets/img/buy-comics-digital-comics.png'
import item2 from '../assets/img/buy-comics-merchandise.png'
import item3 from '../assets/img/buy-comics-subscriptions.png'
import item4 from '../assets/img/buy-comics-shop-locator.png'
import item5 from '../assets/img/buy-dc-power-visa.svg'


export default {
    name: 'SecondContent',
    data () {
        return{
            itemsList: 
            [
                {
                    img: item1,
                    text: 'DIGITAL COMICS',
                }, 
                {
                    img: item2,
                    text: 'DC MERCHANDISE',
                },                
                {
                    img: item3,
                    text: 'SUBSCRIPTION',
                },                
                {
                    img: item4,
                    text: 'COMIC SHOP LOCATOR',
                },                
                {
                    img: item5,
                    text: 'DC POWER VISA',
                },

            ]
        }
    }
}
</script>

<style lang="scss" scoped>
@import "../assets/style/variable.scss";

.container{
    width: 100%;
    height: 150px;
    background-color: $color_bk_primary;
    display: flex;
    align-items: center;
}
.center{
    width: 1200px;
    margin: 0 auto;
}

ul{
    display: flex;
    justify-content: space-between;
    align-items: center;
}

li{
    list-style: none;
    padding: 0 1rem;
    font-size: 15px;

    display: flex;
    align-items: center;

    a{
        margin-left: 10px;
        color: white;
        text-decoration: none;
    }

    img{
        height: 60px;
    }
}
</style>
