<template>
  <div class="container">
      <div class="center">
          <ul>
              <li><img v-for="(element, index) in arrImgList" :key="index" src="" alt="img"><a href="#"></a>{{  }}</li>
          </ul>
      </div>
  </div>
</template>

<script>
export default {
    data () {
        return{
            arrImgList: [
                {
                    img: 'buy-comics-digital-comics.png',
                    text: 'DIGITAL COMICS',
                }
            ]
        }
    }

}
</script>

<style lang="scss" scoped>
.container{
    width: 100vw;
    height: 200px;
    background-color: #255ee9;
}
</style>