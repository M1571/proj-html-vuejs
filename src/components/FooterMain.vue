// ------------------------------------
// HTML

<template>
    
    <footer class="footer">

        <!-- ------------------------------------ -->
        <!-- FOOTER TOP -->

        <div class="footer-top">

            <div class="card-wrapper">
                <div class="card-item uno">
                    <img src="../assets/img/14_Avada_Pet_Supplies/mobile-light-pet-logo-2x.png" width="104px" alt="">
                    <p>1234 Avada Avenue Avadaville</p>
                    <p>info@your-company.com</p>
                    <p>Call us: (1) 234 5678</p>
                </div>
                <div class="card-item due">
                    <h5>Shop by brand</h5>
                    <p>Bed</p>
                    <p>Food</p>
                    <p>Toys</p>
                    <p>Transport</p>
                </div>
                <div class="card-item tre">
                    <h5>Useful links</h5>
                    <p>My account</p>
                    <p>Orders</p>
                    <p>Checkout</p>
                    <p>Cart</p>
                </div>
                <div class="card-item tuscee">
                    <h6>Subscribe to our newsletter</h6>
                    <input type="email" placeholder="Insert your email ...*">
                    <button>Subscribe</button>
                </div>
            </div>  

            <!-- ------------------------------------ -->

            <div class="about-wrapper">

                <div class="lista-nav">
                    <ul>
                        <li>
                            <a href="#">Home</a>
                        </li>
                        <li>
                            <a href="#">About</a>
                        </li>
                        <li>
                            <a href="#">Blog</a>
                        </li>
                        <li>
                            <a href="#">Contact</a>
                        </li>
                        <li>
                            <a href="#">Shop</a>
                        </li>
                    </ul>
                </div>

                <div class="lista-icone">
                    <ul>
                        <li><i class="fa-brands fa-facebook-f"></i></li>
                        <li><i class="fa-brands fa-twitter"></i></li>
                        <li><i class="fa-brands fa-instagram"></i></li>
                        <li><i class="fa-brands fa-youtube"></i></li>
                    </ul>
                </div>
            </div>
        </div>

        <!-- ------------------------------------ -->
        <!-- FOOTER BOTTOM -->

        <div class="footer-bottom">
            <div>
                <p>© Copyright 2012 - 2020 | Avada Theme by ThemeFusion | All Rights Reserved | Powered by @michelangelo_morosi</p>
            </div>
        </div>

        <!-- ------------------------------------ -->

    </footer>

</template>

// ------------------------------------
// JS

<script>

export default {
       
       
       
}

</script>

// ------------------------------------
// CSS

<style lang="scss" scoped>

@import '../assets/scss/_varcolori.scss';

.footer {
    width: 864px;

    .footer-top {
        height: 344px;
        background-color: $main-green;
        display: flex;
        flex-direction: column;
        justify-content: center;
        gap: 30px;

        .card-wrapper {
            border-bottom: 1px solid rgba(212, 212, 212, 0.1);
            width: 616px;
            height: 164px;
            display: flex;

            .card-item {
                width: calc( 616px / 4);
                height: 136px;
                // border: 1px solid red;
                color: white;
                
                p {
                    font-size: 0.5rem;
                    padding: 1px;
                }
            }

            .uno {
                img {
                    margin-bottom: 10px;
                }
            }

            .due {
                h5 {
                    margin-bottom: 10px;
                }

                p {
                    margin-bottom: 10px;
                }
            }

            .tre {
                h5 {
                    margin-bottom: 10px;
                }

                p {
                    margin-bottom: 10px;
                }
            }

            .tuscee {
                height: 135px;
                width: 135px;
                background-color: #264229;
                background-image: url('../assets/img/00_Zampe_background/bg-transparent-3.png');
                // background-position: center;
                background-size: 140%;
                display: flex;
                flex-direction: column;
                justify-content: center;
                gap: 15px;
                text-align: center;

                input {
                    width: 105px;
                    padding: 6px 15px;
                    // height: 20px;
                    border-radius: 10px; 
                    font-size: 0.5rem; 
                    background: #F3F4F3;
                    border: 0;     
                }

                button {
                    width: 105px;
                    border-radius: 10px;
                    font-size: 0.5rem;
                    padding: 6px 15px;
                    border: 0;
                    font-weight: 550;
                }

                button:hover {
                    background: #3C6F42;
                    color: white;
                    cursor: pointer;
                }
            }
        }

        // ------------------------------------

        .about-wrapper {
            // border: 1px solid red;
            display: flex;
            flex-direction: column;
            gap: 20px;

            ul {
                display: contents;
            }

            .lista-nav {
                // border: 1px solid yellow;
                color: lightgray;
                display: flex;
                flex-direction: row;
                font-size: 0.5rem;
                gap: 15px;

                li:hover {
                    color: white;
                }
            }

            .lista-icone {
                // border: 1px solid royalblue;
                color: lightgray;
                display: flex;
                flex-direction: row;
                font-size: 0.7rem;
                gap: 12px;

                li {
                    cursor: pointer;
                }
            }
        }  
    }

    // ------------------------------------

    .footer-bottom {
        height: 36px;
        background-color: black;
        color: white;
        font-size: 0.4rem;
        display: flex;
        justify-content: center;
        align-items: center;
    }
}

</style>

// ------------------------------------