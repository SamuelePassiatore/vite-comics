<script>
export default {
    name: 'App Header',
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
        <figure>
            <a href="#"><img src="../assets/img/dc-logo.png" alt="logo"></a>
        </figure>
        <nav>
            <ul>
                <li v-for="section in sections" :key="section.text"><a href="#" :class="{ current: section.current }">
                        {{ section.text }} </a>
                </li>
            </ul>
        </nav>
    </header>
</template>

<style scoped>
header {
    display: flex;
    justify-content: space-between;
    align-items: center;
    height: 100px;
}

header img {
    height: 70px;
}

ul {
    display: flex;
    padding: 0;
}


ul li {
    text-transform: uppercase;
    list-style-type: none;
    font-weight: bold;
}

ul li a {
    color: #303030;
    font-size: 11px;
    padding: 10px;
}

ul li a:hover {
    color: dodgerblue;
}

ul li a.current {
    color: dodgerblue;
    border-bottom: 5px solid dodgerblue;
    padding-bottom: 37px;
}
</style>