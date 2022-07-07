<template>
    <div class="back">
        <div class="container">
            <div class="flex">
                <div>
                    <div class="footer-links">
                        <span class="title">DC COMICS</span>
                        <ul>
                            <li v-for="item, index in dcComics" :key="index">
                                <a href="#">{{item.text}}</a>
                            </li>
                        </ul>
                    </div>
                    <div class="footer-links">
                        <span class="title">SHOP</span>
                        <ul>
                            <li v-for="item, index in shop" :key="index">
                                <a href="#">{{item.text}}</a>
                            </li>
                        </ul>
                    </div>
                </div>
                <div>
                    <div class="footer-links">
                        <span class="title">DC</span>
                        <ul>
                            <li v-for="item, index in dc" :key="index">
                                <a href="#">{{item.text}}</a>
                            </li>
                        </ul>
                    </div>
                </div>
                <div>
                    <div class="footer-links">
                        <span class="title">SITES</span>
                        <ul>
                            <li v-for="item, index in sites" :key="index">
                                <a href="#">{{item.text}}</a>
                            </li>
                        </ul>
                    </div>
                </div>
            </div>
            <div>
                <img class="logo" src="../assets/img/dc-logo-bg.png" alt="logo">
            </div>
        </div>
    </div>
</template>

<script>
import TextData from '../assets/dc-comics-link.json';
import ShopLink from '../assets/shop-link.json';
import DcLinks from '../assets/dc-links.json';
import SitesLink from '../assets/sites-link.json';

export default {
    name: 'FooterCompo',
    data() {
        return {
            dcComics: TextData,
            shop: ShopLink,
            dc: DcLinks,
            sites: SitesLink,
        }
    }
}
</script>

<style lang="scss" scoped>
@import '../style/common.scss';
@import '../style/common.scss';
.back {
    background-image: url('../assets/img/footer-bg.jpg');
    color: white;
    overflow: hidden;
}
.title {
    font-size: 25px;
    line-height: 50px;
}
li {
    color: grey;
    padding: 2px;
}
.footer-links {
    padding: 10px;
    margin: 0 25px;
}
.container {
    display: flex;
    justify-content: space-between;
    .logo {
        width: 64%;
        overflow: hidden;
        transform: scale(135%);
    }
}
</style>