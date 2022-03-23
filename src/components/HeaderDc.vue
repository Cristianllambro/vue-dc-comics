<template>
  <header>
      <div class="container">
          <div class="center">
                <img src="../assets/img/dc-logo.png" alt="dc-logo">
                <ul>
                    <li v-for="(list, index) in arrList" :key="index"><a href="#">{{ list.text }}</a></li>
                </ul>
          </div>
      </div>
  </header>
</template>


<script>
export default {
    name: 'HeaderDC',
    data () {
        return{
            listIndex: 1,

            arrList: 
            [
                {
                    text: 'CHARACTER',
                },
                {
                    text: 'COMICS',
                },
                {
                    text: 'MOVIE',
                },
                {
                    text: 'TV',
                },
                {
                    text: 'GAMES',
                },
                {
                    text: 'COLLECTIBLES',
                },
                {
                    text: 'VIDEOS',
                },
                {
                    text: 'FANS',
                },
                {
                    text: 'NEWS',
                },
                {
                    text: 'SHOP',
                },
            ]

        }
    },
    methods:  {
        activeColor(index){
            this.listIndex == this.arrList[index];
        }
    }
}
</script>

<style lang="scss" scoped>
@import "../assets/style/variable.scss";

    .container{
        width: 100%;
    }
    .center{
        width: 1200px;
        height: 120px;
        margin: 0 auto;
        display: flex;
        justify-content: space-between;
        align-items: center;

        img{
            width: 80px;
        }

        a{
            font-size: 14px;
            font-weight: 700;
            text-decoration: none;
            padding: 0 .8rem;
            color: black;

            &:hover{
                color: $color_primary;
                border-bottom: 4px solid $color_primary;
                padding-bottom: 4rem;
            }

        }

    }

    li{
        display: inline-block;
        
    }

</style>
