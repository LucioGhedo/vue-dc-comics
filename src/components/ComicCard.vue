<template>
    <div class="card">
        <div class="img-container">
            <img :src="comicDetails.thumb" :alt="comicDetails.series">
        </div>
        <p>{{ comicDetails.series }}</p>
    </div>
</template>

<script>
export default {
    name: 'ComicCard',
    props: {
        comicDetails: Object
    }
}
</script>

<style lang="scss" scoped>
p {
    margin-top: 20px;
    height: 0;
}
.card {
    width: 190px;
    margin: 15px;
    margin-top: 30px;
    margin-bottom: 40px ;
    .img-container {
        width: 180px;
        height: 170px;
        overflow: hidden;
    }
}
</style>