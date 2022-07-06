<template>
    <div class="back">
        <div class="container">
            <div class="flex">
                <div>
                    <div class="footer-links">
                        <span class="title">DC COMICS</span>
                        <ul>
                            <li>Characters</li>
                            <li>Comics</li>
                            <li>Movies</li>
                            <li>TV</li>
                            <li>Games</li>
                            <li>Videos</li>
                            <li>News</li>
                        </ul>
                    </div>
                    <div class="footer-links">
                        <span class="title">SHOP</span>
                        <ul>
                            <li>
                                <a href="#">test</a>
                            </li>
                        </ul>
                    </div>
                </div>
                <div>
                    <div class="footer-links">
                        <span class="title">DC</span>
                        <ul>
                            <li>
                                <a href="#">TEST</a>
                            </li>
                        </ul>
                    </div>
                </div>
                <div>
                    <div class="footer-links">
                        <span class="title">SITES</span>
                        <ul>
                            <li>
                                <a href="#">TEST</a>
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
export default {
    name: 'FooterCompo'
}
</script>

<style lang="scss" scoped>
@import url('../style/common.scss');
@import url('../style/common.scss');
.back {
    background-image: url('../assets/img/footer-bg.jpg');
    color: white;
    height: 330px;
    overflow: hidden;
}
.title {
    font-size: 25px;
    line-height: 50px;
}
li {
    color: grey;
}
.footer-links {
    padding: 10px;
}
.container {
    display: flex;
    justify-content: space-between;
    .logo {
        width: 60%;
        overflow: hidden;
    }
}
</style>