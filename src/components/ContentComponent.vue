<template>
    <div class="color">
        <div class="container flex">
            <span>Content Here</span>
        </div>
    </div>
</template>

<script>
export default {
    name: 'ContentComponent'
}
</script>

<style lang="scss" scoped>
@import '../style/colors.scss';
.color {
    background-color: #1c1c1c;
    color: white;
    height: 150px;
    .container {
        height: 100%;
        align-items: center;
        span {
            font-size: 30px;
        }
    }
}
</style>