<script>
import HeaderJumbotron from './HeaderJumbotron.vue';
export default {
    name: 'App Header',
    components: { HeaderJumbotron },
    data() {
        return {
            sections: [
                {
                    text: 'Characters',
                    url: '#',
                    current: false,
                },
                {
                    text: 'Comics',
                    url: '#',
                    current: true,
                },
                {
                    text: 'Movies',
                    url: '#',
                    current: false,
                },
                {
                    text: 'TV',
                    url: '#',
                    current: false,
                },
                {
                    text: 'Games',
                    url: '#',
                    current: false,
                },
                {
                    text: 'Collectibles',
                    url: '#',
                    current: false,
                },
                {
                    text: 'Videos',
                    url: '#',
                    current: false,
                },
                {
                    text: 'Fans',
                    url: '#',
                    current: false,
                },
                {
                    text: 'News',
                    url: '#',
                    current: false,
                },
                {
                    text: 'Shop',
                    url: '#',
                    current: false,
                }
            ]
        }
    }
}
</script>

<template>
    <header class="container">
        <!-- Image -->
        <figure>
            <a href="#"><img src="../assets/img/dc-logo.png" alt="logo"></a>
        </figure>
        <!-- Nav -->
        <nav>
            <ul>
                <li v-for="section in sections" :key="section.text">
                    <a href="#" :class="{ current: section.current }">
                        {{ section.text }}
                    </a>
                </li>
            </ul>
        </nav>
    </header>
    <header-jumbotron></header-jumbotron>
</template>


<style lang="scss" scoped>
@use '../assets/scss/mixins' as *;
@use '../assets/scss/variables' as *;

// Header
header {
    @include flex-center;
    min-height: 100px;

    img {
        height: 70px;
    }
}

// Nav
ul {
    display: flex;
    padding: 0;

    li {
        text-transform: uppercase;
        font-weight: bold;

        a {
            color: $dark-grey;
            font-size: 11px;
            padding: 10px;

            &:hover {
                color: dodgerblue;
            }

            &.current {
                color: dodgerblue;
                border-bottom: 5px solid dodgerblue;
                padding-bottom: 37px;
            }
        }
    }
}
</style>