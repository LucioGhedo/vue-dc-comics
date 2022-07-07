<template>
    <div class="color">
        <div class="container flex">
            <div class="flex-ms" v-for="item, index in bannerContent" :key="index">
                <img v-bind:src="item.img" :alt="item.text">
                <p>{{item.text}}</p>
            </div>
        </div>
    </div>
</template>

<script>
export default {
    name: 'BlueBanner',
    data() {
        return {
            bannerContent: [
                {
                    img: require('../assets/img/buy-comics-digital-comics.png'),
                    text: 'DIGITAL COMICS'
                },
                {
                    img: require('../assets/img/buy-comics-shop-locator.png'),
                    text: 'DC MERCHANDISE'
                },
                {
                    img: require('../assets/img/buy-comics-merchandise.png'),
                    text: 'SUBSCRIPTIONS'
                },
                {
                    img: require('../assets/img/buy-comics-subscriptions.png'),
                    text: 'COMIC SHOP LOCATOR'
                }, 
                {
                    img: require('../assets/img/buy-dc-power-visa.svg'),
                    text:'DC POWER VISA'
                }
            ]
        }
    }
}
</script>

<style lang="scss" scoped>
@import '../style/colors.scss';
@import '../style/common.scss';
.color {
    background-color: $primary;
    height: 140px;
}
.flex-ms {
    display: flex;
    align-items: center;
    img {
        width: 78px;
        padding: 10px;
    }
}
.flex {
        align-items: center;
        height: 100%;
        color: white;
        justify-content: space-evenly;
    }
div {
    img {
        width: 50%;
    }
}
</style>