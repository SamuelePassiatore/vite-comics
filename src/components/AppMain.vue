<script>
export default {
    name: 'App Main',
    data() {
        return {
            text: '--> Content goes here <--',

        }
    }
}
</script>

<template>
    <main>
        <div class="main-top">
            <div class="container">
                <h2>{{ this.text }}</h2>
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
    line-height: 100px;
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