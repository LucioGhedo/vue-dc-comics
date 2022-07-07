<template>
    <div class="jumbo">
        <div class="container">
            <span class="btn">
                CURRENT SERIES
            </span>
        </div>
    </div>
</template>

<script>
export default {
    name: 'UpBanner',
}
</script>

<style lang="scss" scoped>
@import '../style/colors.scss';
@import '../style/common.scss';
.jumbo {
    background-image: url('../assets/img/jumbotron.jpg');
    height: 400px;
    position: relative;
}
.btn {
    background-color: $primary;
    padding: 15px;
    position: absolute;
    bottom: -20px;
    left: 250px;
    font-weight: 700;
    color: white;
}
</style>