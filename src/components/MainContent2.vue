<template>
<div class="item">
    <div class="card-img">
        <img :src="cardImg" :alt="cardSeries">
    </div>
    
    <p class="text-under">{{ cardSeries }}</p>
</div>


</template>

<script>
export default {
    name: 'MainContent2',
    props: {
        cardSeries: String,
        cardImg: String,
    }
}
</script>

<style lang="scss">
.item{
    width: 170px;
    margin: .3rem;    
}

.card-img{

    img{
        width: 150px;
        height: 150px;
        object-fit: cover;
        padding-bottom: .5rem;
    }
}
.text-under{
    font-size: 13px;
    color: white;
    text-transform: uppercase;

    padding-bottom: 2rem;
}
</style>