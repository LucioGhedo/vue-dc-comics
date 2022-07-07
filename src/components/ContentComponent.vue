<template>
    <div class="color">
        <div class="container flex">
            <ComicCard v-for="element, index in comics" :key="index" :comicDetails="element" />
        </div>
        <div class="flex-2">
            <div class="btn">
                LOAD MORE
            </div>
        </div>
    </div>
</template>

<script>
import ComicJson from '../assets/dc-comics.json';
import ComicCard from './ComicCard.vue';
export default {
    name: "ContentComponent",
    components: { 
        ComicCard
        },
    data() {
        return {
            comics: ComicJson
        }
    }
}
</script>

<style lang="scss" scoped>
@import '../style/colors.scss';
@import '../style/common.scss';
.color {
    background-color: #1c1c1c;
    color: white;
    .flex {
        flex-wrap: wrap;
    }
    .container {
        height: 100%;
        align-items: center;
        span {
            font-size: 30px;
        }
    }
}
.flex-2 {
    display: flex;
    justify-content: center;
}
.btn {
    padding: 15px 80px;
    background-color: $primary;
    display: inline-block;
    margin-bottom: 20px;
}

</style>