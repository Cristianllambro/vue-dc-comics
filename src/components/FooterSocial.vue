<template>
  <div class="container">
      <div class="center">
          <button class="btn-foot">SIGN-UP NOW!</button>
          <div class="social">
                <ul>
                    <li class="txt">FOLLOW US</li>
                    <li v-for="element in arrImageSocial" :key="element" >
                        <img :src="element.img" alt="">
                    </li>
                </ul>
          </div>
      </div>
  </div>
</template>

<script>
import item1 from '../assets/img/footer-facebook.png'
import item2 from '../assets/img/footer-twitter.png'
import item3 from '../assets/img/footer-youtube.png'
import item4 from '../assets/img/footer-pinterest.png'
import item5 from '../assets/img/footer-periscope.png'

export default {
    name: 'FooterSocial',
    data () {
        return {
            arrImageSocial: 
            [
                {
                    img: item1
                },                {
                    img: item2
                },                {
                    img: item3
                },                {
                    img: item4
                },                {
                    img: item5
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
    background-color: $color_bk_gray;
}

.center{
    height: 100px;
    width: 1200px;
    margin: 0 auto;
    display: flex;
    justify-content: space-between;
    align-items: center;
}

.btn-foot{
    font-size: 16px;
    background-color: transparent;
    border: 2px solid $color_primary;
    color: white;
    padding: .6rem 1.4rem;
    cursor: pointer;
}

.txt{
    color: $color_primary;
    font-size: 20px;
    font-weight: 700;

    padding-right: 1.3rem;

    display: inline-block;
}

ul{
    display: flex;
    align-items: center;
}

li{
    display: inline-block;
    padding: .5rem;
    cursor: pointer;
}

</style>
