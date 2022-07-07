<template>
    <div class="container">
        <div class="flex">
            <div>
                <img src="../assets/img/dc-logo.png" alt="logo" class="logo">
            </div>
            <div class="navbar">
                <ul class="flex">
                    <li v-for="item, index in menuLink" :key="index" :class="{'active': item.active}" @click="activeSet(index)">
                        <span :class="{'color': item.active}">{{item.text}}</span>
                    </li>
                </ul>
            </div>
        </div>
    </div>
</template>

<script>
export default {
    name: 'PageHeader',
    methods: {
        activeSet(index) {
            if (this.menuLink[index].active) {
                console.log(':)')
            } else {
                for (let i = 0; i < this.menuLink.length; i++) {
                    this.menuLink[i].active = false
                }
                this.menuLink[index].active = true
            }
        }
    },
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
@import '../style/common.scss';
@import '../style/colors.scss';
.logo {
    padding: 10px;
}
li {
    padding: 20px;
    font-weight: 700;
    align-self: center;

    &.active {
        border-bottom: solid $primary 5px;
    }
    
}
.color {
    color: $primary;
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