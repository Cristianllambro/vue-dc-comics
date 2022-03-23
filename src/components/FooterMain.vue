<template>
    <div class="container">
        <div class="center">
            <div class="left">
                <div class="help">
                    <ul>
                        <li class="title">DC COMICS</li>
                        <li v-for="element in arrListFooter1" :key="element" ><a href="">{{ element.text }}</a></li>
                    </ul>

                    <ul>
                        <li class="title">SHOP</li>
                        <li v-for="element in arrListFooter2" :key="element" ><a href="">{{ element.text2 }}</a></li>
                    </ul>
                </div>
                
                <div class="help">
                    <ul>
                        <li class="title">DC</li>
                        <li v-for="element in arrListFooter3" :key="element" ><a href="">{{ element.text3 }}</a></li>
                    </ul>
                </div>

                <div class="help">
                    <ul>
                        <li class="title">SITES</li>
                        <li v-for="element in arrListFooter4" :key="element" ><a href="">{{ element.text4 }}</a></li>
                    </ul>
                </div>
            </div>

            <div class="right"></div>
        </div>
    </div>
</template>

<script>
export default {
    name: 'FooterMain',
    data () {
        return {
            arrListFooter1: 
            [
                {
                    text: 'Characters',
                },
                {
                    text: 'Comics',
                },
                {
                    text: 'Movies',
                },
                {
                    text: 'TV',
                },
                {
                    text: 'Games',
                },
                {
                    text: 'Videos',
                },
                {
                    text: 'News',
                },
            ],

            arrListFooter2: 
            [
                {
                    text2: 'Shop DC',
                },
                {
                    text2: 'Shop DC Collectibles',
                },
            ],

            arrListFooter3: 
            [
                {
                    text3: 'Terms Of Use'
                },
                {
                    text3: 'Privacy policy (New)'
                },
                {
                    text3: 'Ad Choices'
                },
                {
                    text3: 'Advertising'
                },
                {
                    text3: 'Jobs'
                },
                {
                    text3: 'Subscription'
                },
                {
                    text3: 'Talent Workshops'
                },
                {
                    text3: 'CPSC Certificates'
                },
                {
                    text3: 'Ratings'
                },
                {
                    text3: 'Shop Help'
                },
                {
                    text3: 'Contact Us'
                },
            ],

            arrListFooter4:
            [
                {
                    text4: 'DC',
                },
                {
                    text4: 'MAD Magazine',
                },
                {
                    text4: 'DC Kids',
                },
                {
                    text4: 'DC Universe',
                },
                {
                    text4: 'DC Power Visa',
                },
            ]
            
        }
    }
}
</script>

<style lang="scss" scoped>
.container{
    width: 100%;
    height: 470px;
    background-image: url(../assets/img/footer-bg.jpg);
    background-position: center;
    background-size: cover;
}

.center{
    width: 1200px;
    margin: 0 auto;
    display: flex;

}

.left{
    width: 50%;
    display: flex;

    li{
        list-style: none;
        margin: .7rem 0;

        a{
            font-size: 15px;
            text-decoration: none;
            color: grey;
        }
    }

    .help{
        margin-top: 3rem;
        padding-right: 3rem;
    }
}

.right{
    width: 50%;
    height: 470px;
    background-image: url(../assets/img/dc-logo-bg.png);
    overflow-y: hidden;
    background-size: cover;
    background-position: center;
    overflow: hidden;
}
.title{
    font-size: 22px;
    color: white;
}
</style>
