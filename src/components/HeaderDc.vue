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

    .container{
        width: 100%;
    }
    .center{
        width: 1200px;
        height: 150px;
        margin: 0 auto;
        display: flex;
        justify-content: space-between;
        align-items: center;

        a{
            font-size: 14px;
            text-decoration: none;
            padding: 0 .8rem;
            color: black;
        }

        a:hover{
            color: #255ee9;
        }
    }

    li{
        display: inline-block;
    }

</style>