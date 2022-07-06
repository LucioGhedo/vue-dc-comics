<template>
    <div class="color">
        <div class="container flex">
            <div class="flex-ms">
                <img src="../assets/img/buy-comics-digital-comics.png" alt="buy">
                <p>DIGITAL COMICS</p>
            </div>
            <div class="flex-ms">
                <img src="../assets/img/buy-comics-shop-locator.png" alt="buy">
                <p>DC MERCHANDISE</p>
            </div>
            <div class="flex-ms">
                <img src="../assets/img/buy-comics-merchandise.png" alt="buy">
                <p>SUBSCRIPTIONS</p>
            </div>
            <div class="flex-ms">
                <img src="../assets/img/buy-comics-subscriptions.png" alt="buy">
                <p>COMIC SHOP LOCATOR</p>
            </div>
            <div class="flex-ms">
                <img src="../assets/img/buy-dc-power-visa.svg" alt="buy">
                <p>DC POWER VISA</p>
            </div>
        </div>
    </div>
</template>

<script>
export default {
    name: 'BlueBanner'
}
</script>

<style lang="scss" scoped>
@import url('../style/colors.scss');
@import url('../style/common.scss');
.color {
    background-color: #2481f4;
    height: 120px;
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