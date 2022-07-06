<template>
    <div class="back">
        <div class="container">
            <div class="flex">
                <div>
                    <div class="footer-links">
                        <span class="title">DC COMICS</span>
                        <ul>
                            <li v-for="link in dcComics" :key="link">
                                <a href="#">{{link.text}}</a>
                            </li>
                            <!-- <li>Comics</li>
                            <li>Movies</li>
                            <li>TV</li>
                            <li>Games</li>
                            <li>Videos</li>
                            <li>News</li> -->
                        </ul>
                    </div>
                    <div class="footer-links">
                        <span class="title">SHOP</span>
                        <ul>
                            <li v-for="link in shop" :key="link">
                                <a href="#">{{link.text}}</a>
                            </li>
                        </ul>
                    </div>
                </div>
                <div>
                    <div class="footer-links">
                        <span class="title">DC</span>
                        <ul>
                            <li v-for="link in dc" :key="link">
                                <a href="#">{{link.text}}</a>
                            </li>
                        </ul>
                    </div>
                </div>
                <div>
                    <div class="footer-links">
                        <span class="title">SITES</span>
                        <ul>
                            <li v-for="link in sites" :key="link">
                                <a href="#">{{link.text}}</a>
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
    name: 'FooterCompo',
    data() {
        return {
            dcComics: [
                {
                    text: 'Characters',
                    active: false
                },
                {
                    text: 'Comics',
                    active: false
                },
                {
                    text: 'Movies',
                    active: false
                }, 
                {
                    text: 'TV',
                    active: false
                },
                {
                    text: 'Games',
                    active: false
                },
                {
                    text: 'Videos',
                    active: false
                },
                {
                    text: 'News',
                    active: false
                }
            ],
            shop: [
                {
                    text: 'Shop DC',
                    active: false
                }, 
                {
                    text: 'Shop DC Collectibles',
                    active: false
                }
            ],
            dc: [
                {
                    text: 'Terms Of Use',
                    active: false
                }, 
                {
                    text: 'Privacy Policy (New)',
                    active: false
                },
                {
                    text: 'Ad Choices',
                    active: false
                },
                {
                    text: 'Adversiting',
                    active: false
                },
                {
                    text: 'Jobs',
                    active: false
                },
                {
                    text: 'Subscriptions',
                    active: false
                },
                {
                    text: 'Talent Workshop',
                    active: false
                },
                {
                    text: 'CPSC Certificates',
                    active: false
                },
                {
                    text: 'Ratings',
                    active: false
                },
                {
                    text: 'Shop Help',
                    active: false
                },
                {
                    text: 'Contact Us',
                    active: false
                }
            ],
            sites: [
                {
                    text: 'DC',
                    active: false
                },
                {
                    text: 'MAD Magazine',
                    active: false
                },
                {
                    text: 'DC Kids',
                    active: false
                },
                {
                    text: 'DC Universe',
                    active: false
                },
                {
                    text: 'DC Power Visa',
                    active: false
                },
            ]
        }
    }
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
        width: 60%;
        overflow: hidden;
    }
}
</style>