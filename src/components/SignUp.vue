<template>
    <div class="color">
        <div class="container">
            <div class="flex">
                <div>
                    <div class="btn">SIGN UP NOW!</div>
                </div>
                <div class="flex">
                    <div class="weight">FOLLOW US!</div>
                    <div class="flex">
                        <img src="../assets/img/footer-facebook.png" alt="fb">
                        <img src="../assets/img/footer-periscope.png" alt="fb">
                        <img src="../assets/img/footer-pinterest.png" alt="fb">
                        <img src="../assets/img/footer-twitter.png" alt="fb">
                        <img src="../assets/img/footer-youtube.png" alt="fb">
                    </div>
                </div>
            </div>
        </div>
    </div>
</template>

<script>
export default {
    name: 'SignUp'
}
</script>

<style lang="scss" scoped>
@import url('../style/common.scss');
.color {
    background-color: #303030;
    color: white;
    height: 100px;
    .container {
        height: 100%;
    }
}
.flex {
    justify-content: space-between;
    align-items: center;
    height: 100%;
    img {
        padding: 10px;
    }
}
.btn {
    padding: 15px;
    border: solid #2481f4 1px;
}
.weight {
    font-weight: 800;
    color: #2481f4;
}
</style>