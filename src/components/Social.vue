<template>
    <div>
        <div class="container">
            <div class="signup">
                <a href="/">Sign-Up Now!</a>
            </div>
            <ul class="social">
                <li>
                    <a href="/">Follow Us</a>
                </li>
                <li>
                    <a href="/">
                        <img src="../assets/footer-facebook.png" alt="Facebook">
                    </a>
                </li>
                <li>
                    <a href="/">
                        <img src="../assets/footer-twitter.png" alt="Twitter">
                    </a>
                </li>
                <li>
                    <a href="/">
                        <img src="../assets/footer-youtube.png" alt="Youtube">
                    </a>
                </li>
                <li>
                    <a href="/">
                        <img src="../assets/footer-pinterest.png" alt="Pinterest">
                    </a>
                </li>
                <li>
                    <a href="/">
                        <img src="../assets/footer-periscope.png" alt="Periscope">
                    </a>
                </li>
            </ul>
        </div>
    </div>
</template>

<script>
export default {
    name: 'Social',
}
</script>

<style scoped lang="scss">
div {
    background: #303030;

    .container {
        display: flex;
        align-items: center;
        padding: 30px 0;

        .signup {
            a {
                display: block;
                padding: 10px 20px;
                border: 3px solid #0282f9;
                font-size: 24px;
                font-weight: 700;
                color: #fff;
                text-decoration: none;
                text-transform: uppercase;
            }
        }

        ul.social {
            display: flex;
            justify-content: flex-end;
            align-items: center;
            flex-grow: 1;
            list-style: none;

            li {
                margin: 0 10px;
            }

            a {
                font-size: 24px;
                font-weight: 700;
                color: #0282f9;
                text-decoration: none;
                text-transform: uppercase;
            }
        }
    }
}
</style>