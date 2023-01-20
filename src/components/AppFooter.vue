<script>
export default {
    name: 'App Footer',
    data() {
        return {
        }
    }
}
</script>

<template>
    <footer>
        <div class="container">
            <div class="footer-button"><button>SIGN-UP NOW!</button></div>
            <div class="footer-icons">
                <div class="footer-text">FOLLOW US</div>
                <div class="footer-social">
                    <ul>
                        <li>
                            <a href="#"><img src="../assets/img/footer-facebook.png" alt="facebook"></a>
                            <a href="#"><img src="../assets/img/footer-twitter.png" alt="twitter"></a>
                            <a href="#"><img src="../assets/img/footer-youtube.png" alt="you-tube"></a>
                            <a href="#"><img src="../assets/img/footer-pinterest.png" alt="pinterest"></a>
                            <a href="#"><img src="../assets/img/footer-periscope.png" alt="maps"></a>
                        </li>
                    </ul>
                </div>
            </div>
        </div>
    </footer>
</template>

<style scoped>
footer {
    min-height: 100px;
    background-color: #303030;
}

footer .container {
    display: flex;
    height: 100px;
    justify-content: space-between;
    align-items: center;
}

.footer-button button {
    padding: 10px 10px;
    background-color: transparent;
    color: white;
    border-color: dodgerblue;
    cursor: pointer;
}

.footer-icons {
    display: flex;
}

.footer-icons .footer-text {
    display: flex;
    align-items: center;
    color: dodgerblue;
    font-weight: bold;
    padding: 0 20px;
    cursor: pointer;
}

.footer-icons .footer-social li {
    display: flex;
}

.footer-icons .footer-social li img {
    padding: 0 5px;
}
</style>