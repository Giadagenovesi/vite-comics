<script>
export default {
    name: "AppFooter",
}
</script>

<template>
    <footer>
        <div class="footer-top">
            <div class="container">
                <div class="shop-links">
                    <ul>
                        <li>
                            <img src="../assets/img/buy-comics-digital-comics.png" alt="dc logo bg">
                            <p>DIGITAL COMICS</p>
                        </li>
                        <li>
                            <img src="../assets/img/buy-comics-merchandise.png" alt="dc logo bg">
                            <p>DIGITAL COMICS</p>  
                        </li>
                        <li>
                            <img src="../assets/img/buy-comics-subscriptions.png" alt="dc logo bg">
                            <p>DIGITAL COMICS</p>  
                        </li>
                        <li>
                            <img src="../assets/img/buy-comics-shop-locator.png" alt="dc logo bg">
                            <p>DIGITAL COMICS</p>  
                        </li>
                        <li>
                            <img src="../assets/img/buy-dc-power-visa.svg" alt="dc logo bg">
                            <p>DIGITAL COMICS</p>  
                        </li>
                    </ul>    
                </div>
            </div>     
        </div>
        
        <div class="main-footer">
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
            <div class="container">
                <div class="sign-btn">
                    <a href="">SIGN-UP NOW!</a>
                </div>
                <nav class="socials">
                    <h3>FOLLOW US</h3>
                    <a href="">
                        <img src="../assets/img/footer-facebook.png" alt="fb logo">
                    </a>
                    <a href="">
                        <img src="../assets/img/footer-twitter.png" alt="twitter logo">
                    </a>
                    <a href="">
                        <img src="../assets/img/footer-youtube.png" alt="youtube logo">
                    </a>
                    <a href="">
                        <img src="../assets/img/footer-pinterest.png" alt="pinterest logo">
                    </a>
                    <a href="">
                        <img src="../assets/img/footer-periscope.png" alt="location logo">
                    </a>
                </nav>
            </div>
        </div>
    </footer>
</template>

<style scoped lang="scss">
@use "../style/partials/mixins" as *;

footer {
    background-size: cover;
    background-image: url(../assets/img/footer-bg.jpg);

    .footer-top {
        background-color: #0282F9;
        padding: 2rem 0

    }
    .container {
        @include flex (row, space-between, center);
        

        .shop-links {
            display: flex;
            color: white;
            padding-left: 2rem;

            ul {
                display: flex;
                list-style-type: none;


                li {
                    display: flex;
                    align-items: center;
                    justify-content: space-around;

                    img {
                        width: 40px;
                        margin:0  10px;
                    }
                    p {
                        margin-right: 30px;
                        font-size: .8rem;
                    }
                }
            }
        }
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
   
    .footer-bottom {
        width: 100%;
        height: 100px;
        background-color: #303030;
        padding: 1.5rem 0;
        display: flex;
        align-items: center;
        
        .sign-btn {
            padding: 1rem .6rem;
            border: 3px solid #0282F9;
            
            a {
                color: white;
                text-decoration: none;
            }
        }
        h3 {
            color: #0282F9;
            margin-right: 1rem;
        }
        
        .socials {
            display: flex;
            align-items: center;

            a {
                width: 28px;
                margin: 0 .3rem;
            }
        }
    }
}
</style>