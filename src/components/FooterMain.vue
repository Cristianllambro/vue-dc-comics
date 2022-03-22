<template>
    <div class="container">
        <div class="center">
            <div class="left">

            </div>

            <!-- <div class="right"><img src="../assets/img/dc-logo-bg.png" alt=""></div> -->
        </div>
    </div>
</template>

<script>
export default {
    data () {
        return {
            arrListFooter: 
            [
                {

                }
            ]
        }
    }
}
</script>

<style lang="scss" scoped>
.container{
    width: 100%;
    height: 400px;
    background-image: url(../assets/img/footer-bg.jpg);
    object-fit: cover;
    background-position: center;
}

.right{
    width: 50%;

    img{
        display: inline-block;
    }
}
</style>