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

        </div>

        <div class="main-bottom">
            <div class="container">
                <div class="main-list">
                    <ul>
                        <li class="title-list">DC COMICS</li>
                        <li>Characters</li>
                        <li>Comics</li>
                        <li>Movie</li>
                        <li>TV</li>
                        <li>Games</li>
                        <li>Videos</li>
                        <li>News</li>
                        <li class="title-list">SHOP</li>
                        <li>Shop DC</li>
                        <li>Shop DC Collections</li>
                    </ul>
                    <ul>
                        <li class="title-list">DC</li>
                        <li>Terms of use</li>
                        <li>Privacy policy (New)</li>
                        <li>Ad choices</li>
                        <li>Advertising</li>
                        <li>Jobs</li>
                        <li>Subscriptions</li>
                        <li>Talent Workshop</li>
                        <li>CPSC Certificates</li>
                        <li>Ratings</li>
                        <li>Shop Help</li>
                        <li>Contact Us</li>
                    </ul>
                    <ul>
                        <li class="title-list">SITES</li>
                        <li>DC</li>
                        <li>MAD Magazine</li>
                        <li>DC Kids</li>
                        <li>DC Universe</li>
                        <li>DC Power Visa</li>
                    </ul>
                </div>
                <div class="main-img"></div>
            </div>
        </div>
    </main>
</template>

<style scoped>
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
}

/* Main bottom */
.main-bottom {
    min-height: 300px;
    background-image: url('../assets/img/footer-bg.jpg');
    background-size: cover;
    background-repeat: no-repeat;
}

.main-bottom .container {
    display: flex;
}

/* Main bottom list */
.main-bottom .main-list {
    flex-basis: 50%;
    display: flex;
    padding: 20px 0;
}

.main-bottom .main-list ul {
    display: flex;
    flex-direction: column;
    padding: 0 15px;
}

.main-bottom li {
    color: grey;
    font-size: 13px;
    padding: 2px;
}

.main-bottom li.title-list {
    font-size: 20px;
    color: white;
    text-transform: uppercase;
    padding: 10px 0;
}

/* Main bottom img */
.main-bottom .main-img {
    flex-basis: 50%;
    min-height: 300px;
    background-image: url('../assets/img/dc-logo-bg.png');
    background-position: center;
    background-size: cover;
    background-repeat: no-repeat;
}
</style>