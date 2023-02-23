<script>
import SeriesCard from './SeriesCard.vue'
import AppButton from './AppButton.vue'
export default {
    name: 'App Main',
    components: { SeriesCard, AppButton },
    data() {
        return {
            text: 'CURRENT SERIES',
            cards: [
                {
                    thumb:
                        'https://imgs.search.brave.com/aUNyvZBXUulb963JH7KnQm9AMr8bcBoLsiHREOqayIU/rs:fit:612:612:1/g:ce/aHR0cHM6Ly9pNS53/YWxtYXJ0aW1hZ2Vz/LmNvbS9hc3IvOWZm/ZWYzMDMtMGZhYy00/OGRkLTg3ODctYzUy/NTk0MDk2ODAwXzEu/MTc1ZDk1Mjg2NzY0/OGEwOTczMTY2NGMy/MTE1NjNlYWIuanBl/Zz9vZG5XaWR0aD02/MTImb2RuSGVpZ2h0/PTYxMiZvZG5CZz1m/ZmZmZmY',
                    price: '$19.99',
                    series: 'Action Comics',
                    type: 'comic book',
                },
                {
                    thumb:
                        'https://imgs.search.brave.com/OU2E3_3vA7flyv-SJ3TcFW1d99KDlp5ZfmW9ylLLFDo/rs:fit:1012:1200:1/g:ce/aHR0cHM6Ly9pMC53/cC5jb20vd3d3LnN1/cGVycG91dm9pci5j/b20vd3AtY29udGVu/dC91cGxvYWRzLzIw/MjAvMDcvQW1lcmlj/YW4tVmFtcGlyZS0x/OTc2LTAxLWNvdi1B/bGJ1cXVlcnF1ZS0y/MDIwLmpwZz9yZXNp/emU9MTAxMiUyQzE1/NTYmc3NsPTE',
                    price: '$3.99',
                    series: 'American Vampire 1976',
                    type: 'comic book',
                },
                {
                    thumb:
                        'https://imgs.search.brave.com/gAZQuZyt6WjcUWF6aXCIBaiJqtOJAK-X4nxS9Vbvwno/rs:fit:1200:1200:1/g:ce/aHR0cHM6Ly9jZG4y/LnBlbmd1aW4uY29t/LmF1L2NvdmVycy9v/cmlnaW5hbC85Nzgx/NDAxMjc1NDI2Lmpw/Zw',
                    price: '$16.99',
                    series: 'Aquaman',
                    type: 'graphic novel',
                },
                {
                    thumb:
                        'https://imgs.search.brave.com/YET9wY29Aa29TyHqlbieS9qsz3HWyNYQx-WkRqdBRX4/rs:fit:640:984:1/g:ce/aHR0cDovL2dldHlv/dXJjb21pY29uLmNv/LnVrL3dwLWNvbnRl/bnQvdXBsb2Fkcy8y/MDE2LzA4L2JhdGdp/cmwtcmViaXJ0aC0x/LWNvdmVyLmpwZw',
                    price: '$2.99',
                    series: 'Batgirl',
                    type: 'comic book',
                },
                {
                    thumb:
                        'https://imgs.search.brave.com/jgxYlrx442aozemzjqdmCsd9DkIkRollJp1T8sG8TfE/rs:fit:720:1106:1/g:ce/aHR0cHM6Ly9veXN0/ZXIuaWduaW1ncy5j/b20vd29yZHByZXNz/L3N0Zy5pZ24uY29t/LzIwMTgvMTAvU1RM/MDk3MDk1LTcyMHgx/MTA2LmpwZw',
                    price: '$3.99',
                    series: 'Batman',
                    type: 'comic book',
                },
                {
                    thumb:
                        'https://imgs.search.brave.com/jgxYlrx442aozemzjqdmCsd9DkIkRollJp1T8sG8TfE/rs:fit:720:1106:1/g:ce/aHR0cHM6Ly9veXN0/ZXIuaWduaW1ncy5j/b20vd29yZHByZXNz/L3N0Zy5pZ24uY29t/LzIwMTgvMTAvU1RM/MDk3MDk1LTcyMHgx/MTA2LmpwZw',
                    price: '$2.99',
                    series: 'Batman Beyond',
                    type: 'comic book',
                },
                {
                    thumb:
                        'https://imgs.search.brave.com/cSaB3m-tghN3_Cllp9IOlUPEPsyShCnl8gijRyPFdrg/rs:fit:791:1200:1/g:ce/aHR0cHM6Ly8xNDk0/NTUxNTIudjIucHJl/c3NhYmxlY2RuLmNv/bS93cC1jb250ZW50/L3VwbG9hZHMvMjAx/OS8wOC9CTVNNX0N2/MV9CQVQuanBn',
                    price: '$3.99',
                    series: 'Batman/Superman',
                    type: 'comic book',
                },
                {
                    thumb:
                        'https://imgs.search.brave.com/jfaQd--WUx7RG8MiQ-VyCOqLUJW19ojBnjkNOG81rL4/rs:fit:666:1024:1/g:ce/aHR0cHM6Ly90aGVn/d3cuY29tL3dwLWNv/bnRlbnQvdXBsb2Fk/cy8yMDIwLzA5L0Jh/dG1hbi1TdXBlcm1h/bi1Bbm51YWwtQ3Yx/LTY2NngxMDI0Lmpw/Zw',
                    price: '$4.99',
                    series: 'Batman/Superman Annual',
                    type: 'comic book',
                },
                {
                    thumb:
                        'https://imgs.search.brave.com/kSLCPBIeE9s218LRC4cIyrHOYmxrSS2Wt7LvNNfED2I/rs:fit:455:700:1/g:ce/aHR0cHM6Ly9jb21p/Y2Jvb2tyZWFsbS5j/b20vY292ZXItc2Nh/bi81ZmFmMTFjYTk1/NGQ1MGVjZDA1ZmU3/M2U1NjBiNWQyOC94/bC8tLWlzc3VlLTEu/anBn',
                    price: '$5.99',
                    series: 'Batman: The Joker War Zone',
                    type: 'comic book',
                },
                {
                    thumb:
                        'https://imgs.search.brave.com/a6fAPUra4t94xMJFlYv6X7Lwm4z_qPmslx7Hiqafbok/rs:fit:600:923:1/g:ce/aHR0cHM6Ly9jZG4u/ZmxpY2tlcmluZ215/dGguY29tL3dwLWNv/bnRlbnQvdXBsb2Fk/cy8yMDIwLzA4L0Jh/dG1hbi1UaHJlZS1K/b2tlcnMtMS02MDB4/OTIzLTEuanBn',
                    price: '$6.99',
                    series: 'Batman: Three Jokers',
                    type: 'comic book',
                },
                {
                    thumb:
                        'https://imgs.search.brave.com/qMxyCwK99aguaETp4ioxXLrpxwNg2JNBN3Oq7LGAgzM/rs:fit:780:1200:1/g:ce/aHR0cHM6Ly9jZG4u/ZmxpY2tlcmluZ215/dGguY29tL3dwLWNv/bnRlbnQvdXBsb2Fk/cy8yMDIwLzEwL0Jh/dG1hbi1XaGl0ZS1L/bmlnaHQtUHJlc2Vu/dHMtSGFybGV5LVF1/aW5uLTEtMS5qcGc',
                    price: '$4.99',
                    series: 'Batman: White Knight Presents: Harley Quinn',
                    type: 'comic book',
                },
                {
                    thumb:
                        'https://imgs.search.brave.com/bf_FlGnymAgmvweY8YiLAcyy600JdSMl_jHpdR3t5ro/rs:fit:612:612:1/g:ce/aHR0cHM6Ly9pNS53/YWxtYXJ0aW1hZ2Vz/LmNvbS9hc3IvNTA5/M2IxOTEtZTkzZS00/NTJjLThhYTQtYTEw/ZDY0ZTcxN2E5LjA5/N2UwZWM5NDgzYzky/OGExMjY4Nzk1Nzk2/NTliZWNjLmpwZWc_/b2RuV2lkdGg9NjEy/Jm9kbkhlaWdodD02/MTImb2RuQmc9ZmZm/ZmZm',
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
                <div class="button">
                    <app-button text="Load More"></app-button>
                </div>
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
    padding-bottom: 20px;

    h2 {
        display: inline-block;
        background-color: dodgerblue;
        padding: 5px 10px;
        font-size: 18px;
        text-transform: uppercase;
        position: relative;
        bottom: 18px;
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