// ------------------------------------
// HTML

<template>
    
    <footer class="footer">

        <!-- ------------------------------------ -->
        <!-- FOOTER TOP -->

        <div class="footer-top">

            <div class="card-wrapper">
                <div class="card-item uno">1</div>
                <div class="card-item due">2</div>
                <div class="card-item tre">3</div>
                <div class="card-item tuscè">4</div>
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
            border: 1px solid royalblue;
            width: 616px;
            height: 164px;
            display: flex;

            .card-item {
                width: calc( 616px / 4);
                border: 1px solid red;
            }
        }

        // ------------------------------------

        .about-wrapper {
            border: 1px solid red;
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