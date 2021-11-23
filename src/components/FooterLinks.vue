<template>
    <div>
        <div class="container">
            <div>
                <h4>DC Comics</h4>
                <ul>
                    <li>
                        <a href="/">Characters</a>
                    </li>
                    <li>
                        <a href="/">Comics</a>
                    </li>
                    <li>
                        <a href="/">Movies</a>
                    </li>
                    <li>
                        <a href="/">TV</a>
                    </li>
                    <li>
                        <a href="/">Games</a>
                    </li>
                    <li>
                        <a href="/">Videos</a>
                    </li>
                    <li>
                        <a href="/">News</a>
                    </li>
                </ul>
                <h4>Shop</h4>
                <ul>
                    <li>
                        <a href="/">Shop DC</a>
                    </li>
                    <li>
                        <a href="/">Shop DC Collectibles</a>
                    </li>
                </ul>
            </div>

            <div>
                <h4>DC</h4>
                <ul>
                    <li>
                        <a href="/">Terms Of Use</a>
                    </li>
                    <li>
                        <a href="/">Privacy Policy (New)</a>
                    </li>
                    <li>
                        <a href="/">Ad Choices</a>
                    </li>
                    <li>
                        <a href="/">Advertising</a>
                    </li>
                    <li>
                        <a href="/">Jobs</a>
                    </li>
                    <li>
                        <a href="/">Subscriptions</a>
                    </li>
                    <li>
                        <a href="/">Talent Workshops</a>
                    </li>
                    <li>
                        <a href="/">CPSC Certificates</a>
                    </li>
                    <li>
                        <a href="/">Ratings</a>
                    </li>
                    <li>
                        <a href="/">Shop Help</a>
                    </li>
                    <li>
                        <a href="/">Contact Us</a>
                    </li>
                </ul>
            </div>

            <div>
                <h4>Sites</h4>
                <ul>
                    <li>
                        <a href="/">DC</a>
                    </li>
                    <li>
                        <a href="/">MAD Magazine</a>
                    </li>
                    <li>
                        <a href="/">DC Kids</a>
                    </li>
                    <li>
                        <a href="/">DC Universe</a>
                    </li>
                    <li>
                        <a href="/">DC Power Visa</a>
                    </li>
                </ul>
            </div>

        </div>
    </div>
</template>

<script>
export default {
    name: 'FooterLinks',
}
</script>

<style scoped lang="scss">
div {
    background-image: url('../assets/footer-bg.jpg');
    background-repeat: no-repeat;
    background-size: cover;

    .container {
        background-image: url('../assets/dc-logo-bg.png');
        background-repeat: no-repeat;
        background-position: center right;
        background-size: 50%;
        padding: 50px 0;
        display: flex;

        div {
            background: transparent;
            margin-right: 30px;

            h4 {
                margin-bottom: 10px;
                color: #fff;
                font-size: 20px;
                font-weight: 700;
                text-transform: uppercase;
            }

            ul {
                list-style: none;
                margin-bottom: 30px;

                li {
                    margin-bottom: 5px;

                    a {
                        color: #959595;
                        font-size: 14px;
                        text-decoration: none;
                    }
                }
            }
        }
    }
}

</style>