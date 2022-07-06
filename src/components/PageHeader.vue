<template>
    <div class="container">
        <div class="flex">
            <div>
                <img src="../assets/img/dc-logo.png" alt="logo" class="logo">
            </div>
            <div class="navbar">
                <ul class="flex">
                    <li v-for="link in menuLink" :key="link" :class="{'active': link.active}">
                        <span :class="{'color': link.active}">{{link.text}}</span>
                    </li>
                </ul>
            </div>
        </div>
    </div>
</template>

<script>
export default {
    name: 'PageHeader',
    data() {
        return {
            menuLink: [
                {
                    text: 'CHARACTERS',
                    active: false
                },
                {
                    text: 'COMICS',
                    active: true
                },
                {
                    text: 'MOVIES',
                    active: false
                },
                {
                    text: 'TV',
                    active: false
                },
                {
                    text: 'GAMES',
                    active: false
                },
                {
                    text: 'COLLECTIBLES',
                    active: false
                },
                {
                    text: 'VIDEOS',
                    active: false
                },
                {
                    text: 'FANS',
                    active: false
                },
                {
                    text: 'NEWS',
                    active: false
                },
                {
                    text: 'SHOP',
                    active: false
                },
            ]
        }
    }
}
</script>

<style lang="scss" scoped>
@import url('../style/common.scss');
@import url('../style/colors.scss');
.logo {
    padding: 10px;
}
li {
    padding: 20px;
    font-weight: 700;
    align-self: center;

    &.active {
        border-bottom: solid #2481f4 5px;
    }
    
}
.color {
    color: #2481f4;
}
ul {
    height: 100%;
    line-height: 82px;
}
.container {
    .flex {
        justify-content: space-between;
    }
}
</style>