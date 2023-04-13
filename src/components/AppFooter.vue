<script>
export default {
    name: "AppFooter",
}
</script>

<template>
    <footer>
        <div class="footer-top">
            <div class="container">
                <div class="footer-menu">
                    <div class="left">
                        <h3> DC COMICS</h3>
                        <ul>
                            <li>Characters</li>
                            <li>Comics</li>
                            <li>Movies</li>
                            <li>TV</li>
                            <li>Games</li>
                            <li>Videos</li>
                            <li>News</li>
                        </ul>
                        <h3> SHOP</h3>
                        <ul>
                            <li>Shop DC</li>
                            <li>Shop DC Collectibles</li>
                        </ul>
                    </div>
                    <div class="center">
                        <h3> DC</h3>
                        <ul>
                            <li>Terms Of Use</li>
                            <li>Privacy policy (New)</li>
                            <li>Ad Choices</li>
                            <li>Advertising</li>
                            <li>Jobs</li>
                            <li>Subscriptions</li>
                            <li>Talent Workshops</li>
                            <li>CPSC Certificates</li>
                            <li>Ratings</li>
                            <li>Shop Help</li>
                            <li>Contact Us</li>
                        </ul>
                    </div>
                    <div class="right">
                        <h3> SITES</h3>
                        <ul>
                            <li>DC</li>
                            <li>MAD Magazine</li>
                            <li>DC Kids</li>
                            <li>DC Universe</li>
                            <li>DC Power Visa</li>    
                        </ul>
                    </div> 
                </div>
                <div class="footer-bg">
                    <img src="../assets/img/dc-logo-bg.png" alt="dc logo bg">
                </div>
            </div>
        </div>
        <div class="footer-bottom">

        </div>
        
    </footer>
</template>

<style scoped lang="scss">
@use "../style/partials/mixins" as *;

footer {
    background-size: cover;
    background-image: url(../assets/img/footer-bg.jpg);

    .container {
        @include flex (row, space-between, center);
        .footer-menu {
            width: 40%;
            align-self: flex-start;
            padding-top: 1.5rem;
            @include flex (row, space-between, center);
            
            h3 {
                margin-bottom: 1rem;
                color: white;
            }
            ul {
                margin-bottom: 1rem;
            }
            li {
                list-style: none;
                font-size: .9rem;
                margin: .4rem 0;
                color: rgb(255, 255, 255, 0.5);
            }
            .right,
            .center {
                align-self: flex-start;
            }
        }
        .footer-bg {
            width: 400px;
        }


    }
    .footer-top {
        padding: 1rem 0;
    }
    .footer-bottom {
        height: 80px;
        background-color: #303030;
        padding: 1.5rem 0; 
    }
}
</style>