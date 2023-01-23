<script>
import SeriesCard from './SeriesCard.vue'
export default {
    name: 'App Main',
    components: { SeriesCard },
    data() {
        return {
            text: 'CURRENT SERIES',
            cards: [
                {
                    thumb:
                        'https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2018/09/AC1000_DLX_162-001_HD_5ba13723281ab0.37845353.jpg?itok=ZsI-C5eX',
                    price: '$19.99',
                    series: 'Action Comics',
                    type: 'comic book',
                },
                {
                    thumb:
                        'https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2020/09/AV1976_01_300-001_HD_5f738f6e39ddd7.18205602.jpg?itok=VgdYdJ01',
                    price: '$3.99',
                    series: 'American Vampire 1976',
                    type: 'comic book',
                },
                {
                    thumb:
                        'https://www.dccomics.com/sites/default/files/styles/covers192x291/public/gn-covers/2018/08/AQMv4_UW_153-001_HD_5b7efa1745a9b8.08589135.jpg?itok=HPTtnrsb',
                    price: '$16.99',
                    series: 'Aquaman',
                    type: 'graphic novel',
                },
                {
                    thumb:
                        'https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2018/06/batgirl_v5_1_5b23e1f1124941.50950783.jpg?itok=VnrJah76',
                    price: '$2.99',
                    series: 'Batgirl',
                    type: 'comic book',
                },
                {
                    thumb:
                        'https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2018/09/BM_56_300-001_HD_5ba137a85c3bf3.33122291.jpg?itok=3FHJQYJZ',
                    price: '$3.99',
                    series: 'Batman',
                    type: 'comic book',
                },
                {
                    thumb:
                        'https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2018/09/BM_56_300-001_HD_5ba137a85c3bf3.33122291.jpg?itok=3FHJQYJZ',
                    price: '$2.99',
                    series: 'Batman Beyond',
                    type: 'comic book',
                },
                {
                    thumb:
                        'https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2019/08/BMSM_5d4361b7116261.74371456.jpg?itok=kEDR2OL8',
                    price: '$3.99',
                    series: 'Batman/Superman',
                    type: 'comic book',
                },
                {
                    thumb:
                        'https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2020/09/BMSMANN_01_300-001_HD_5f5ff17fa1d665.74704970.jpg?itok=azz5sfGk',
                    price: '$4.99',
                    series: 'Batman/Superman Annual',
                    type: 'comic book',
                },
                {
                    thumb:
                        'https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2020/09/BMTJWZ_01_300-001_HD_5f5ff2307dcb37.34652945.jpg?itok=VswVjLR8',
                    price: '$5.99',
                    series: 'Batman: The Joker War Zone',
                    type: 'comic book',
                },
                {
                    thumb:
                        'https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2020/08/cover-v2_5f40314645a734.37285065.png?itok=ImNM2QBY',
                    price: '$6.99',
                    series: 'Batman: Three Jokers',
                    type: 'comic book',
                },
                {
                    thumb:
                        'https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2020/10/BMWK_HQ_01_300-001_HD_5f7cb4945e13f6.89501032.jpg?itok=sVwALbUX',
                    price: '$4.99',
                    series: 'Batman: White Knight Presents: Harley Quinn',
                    type: 'comic book',
                },
                {
                    thumb:
                        'https://www.dccomics.com/sites/default/files/styles/covers192x291/public/gn-covers/2019/04/CTWv1_CC_144-001_HD_5ca5299a751963.53054221.jpg?itok=ooPaoLDq',
                    price: '$16.99',
                    series: 'Catwoman',
                    type: 'graphic novel',
                },
            ]
        }
    }
}
</script>

<template>
    <main>
        <div class="main-top">
            <div class="container">
                <h2>{{ this.text }}</h2>
                <div class="card-container">
                    <series-card v-for="card in cards" :key="card.series" :card="card"></series-card>
                </div>
                <div class="button"><button>LOAD MORE</button></div>
            </div>
        </div>

        <div class="main-center">
            <div class="container">
                <ul>
                    <li>
                        <a href="#">
                            <img src="../assets/img/buy-comics-digital-comics.png" alt="digital">
                            <span>DIGITAL COMICS</span>
                        </a>
                        <a href="#">
                            <img src="../assets/img/buy-comics-merchandise.png" alt="digital">
                            <span>DC MERCHANDISE</span>
                        </a>
                        <a href="#">
                            <img src="../assets/img/buy-comics-subscriptions.png" alt="digital">
                            <span>SUBSCRIPTION</span>
                        </a>
                        <a href="#">
                            <img src="../assets/img/buy-comics-shop-locator.png" alt="digital">
                            <span>COMIC SHOP LOCATOR</span>
                        </a>
                        <a href="#">
                            <img src="../assets/img/buy-dc-power-visa.svg" alt="digital">
                            <span>DC POWER VISA</span>
                        </a>
                    </li>
                </ul>
            </div>
        </div>

        <div class="main-bottom">
            <div class="container">
                <div class="main-list">
                    <ul>
                        <li>
                            <a href="#" class="title-list">DC COMICS</a>
                            <a href="#">Characters</a>
                            <a href="#">Comics</a>
                            <a href="#">Movie</a>
                            <a href="#">TV</a>
                            <a href="#">Games</a>
                            <a href="#">Videos</a>
                            <a href="#">News</a>
                            <a href="#" class="title-list">SHOP</a>
                            <a href="#">Shop DC</a>
                            <a href="#">Shop DC Collections</a>
                        </li>
                    </ul>
                    <ul>
                        <li>
                            <a href="#" class="title-list">DC</a>
                            <a href="#">Terms of use</a>
                            <a href="#">Privacy policy (New)</a>
                            <a href="#">Ad choices</a>
                            <a href="#">Advertising</a>
                            <a href="#">Jobs</a>
                            <a href="#">Subscriptions</a>
                            <a href="#">Talent Workshop</a>
                            <a href="#">CPSC Certificates</a>
                            <a href="#">Ratings</a>
                            <a href="#">Shop Help</a>
                            <a href="#">Contact Us</a>
                        </li>
                    </ul>
                    <ul>
                        <li>
                            <a href="#" class="title-list">SITES</a>
                            <a href="#">DC</a>
                            <a href="#">MAD Magazine</a>
                            <a href="#">DC Kids</a>
                            <a href="#">DC Universe</a>
                            <a href="#">DC Power Visa</a>
                        </li>
                    </ul>
                </div>
                <div class="main-img"></div>
            </div>
        </div>
    </main>
</template>

<style lang="scss" scoped>
/* Main top */
.main-top {
    min-height: 100px;
    background-color: #1C1C1C;
    color: white;
    padding: 20px 0;

    h2 {
        display: inline-block;
        background-color: dodgerblue;
        padding: 5px 10px;
        font-size: 18px;
        text-transform: uppercase;
        position: relative;
        bottom: 38px;
    }

    .card-container {
        display: flex;
        flex-wrap: wrap;

        .series-card {
            flex-basis: calc(100% / 6);
        }
    }

    .button {
        text-align: center;

        button {
            padding: 8px 30px;
            background-color: dodgerblue;
            border: transparent;
            color: white;
        }
    }
}

/* Main center */
.main-center {
    min-height: 120px;
    background-color: dodgerblue;

    ul {
        line-height: 120px;
    }

    li,
    a {
        display: flex;
        justify-content: center;
        align-items: center;
    }

    a {
        flex-basis: calc(100% / 5);

        img {
            width: 50px;
            padding-right: 15px;
        }

        span {
            color: white;
            font-size: 13px;

            &:hover {
                text-shadow: 1px 0 10px white;
            }
        }

    }
}

/* Main bottom */
.main-bottom {
    min-height: 300px;
    background-image: url('../assets/img/footer-bg.jpg');
    background-size: cover;
    background-repeat: no-repeat;

    .container {
        display: flex;
    }

    // Main List
    .main-list {
        flex-basis: 50%;
        display: flex;
        padding: 20px 0;

        ul {
            padding: 0 15px;

            li {
                display: flex;
                flex-direction: column;

                a {
                    color: grey;
                    font-size: 13px;
                    padding: 2px;

                    &:hover {
                        color: white;
                    }
                }

                a.title-list {
                    font-size: 20px;
                    color: white;
                    text-transform: uppercase;
                    padding: 10px 0;

                    &:hover {
                        text-shadow: 1px 0 10px white;
                    }
                }
            }
        }
    }

    // Main img
    .main-img {
        flex-basis: 50%;
        min-height: 300px;
        background-image: url('../assets/img/dc-logo-bg.png');
        background-position: center;
        background-size: cover;
        background-repeat: no-repeat;
    }
}
</style>