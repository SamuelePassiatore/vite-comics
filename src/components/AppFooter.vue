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
            <!-- Footer button -->
            <div class="footer-button"><button>SIGN-UP NOW!</button></div>
            <!-- Footer icons -->
            <div class="footer-icons">
                <!-- Footer icons text -->
                <div class="footer-text">FOLLOW US</div>
                <!-- Footer icons social -->
                <div class="footer-social">
                    <ul>
                        <!-- Images -->
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

<style lang="scss" scoped>
@use '../assets/scss/mixins' as *;
@use '../assets/scss/variables' as *;

// Footer
footer {
    min-height: 100px;
    background-color: $dark-grey;

    .container {
        @include flex-center;
        height: 100px;
    }
}

// Footer button
.footer-button button {
    padding: 10px 10px;
    background-color: transparent;
    color: white;
    border-color: dodgerblue;
    cursor: pointer;

    &:hover {
        box-shadow: inset 1px 0 10px dodgerblue;
    }
}

// Footer icons
.footer-icons {
    display: flex;

    .footer-text {
        display: flex;
        align-items: center;
        color: dodgerblue;
        font-weight: bold;
        padding: 0 20px;
        cursor: pointer;

        &:hover {
            text-shadow: 1px 0 10px dodgerblue;
        }
    }

    .footer-social li {
        display: flex;

        img {
            padding: 0 5px;
        }
    }
}
</style>