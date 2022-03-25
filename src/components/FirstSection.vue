// ------------------------------------
// HTML

<template>

    <section class="section-uno">

        <!-- ------------------------------------ -->
        <!-- TOP -->
    
        <div class="intern-section-top">
            <div class="elements-flex">
                <div class="flex-uno">
                    <i class="fa-solid fa-truck-fast"></i>
                    <p><span>International</span> Shipping Services</p>
                </div>
                <div class="flex-due">
                    <i class="fa-regular fa-clock"></i>
                    <p>See our <span>store hours </span>and services</p>
                </div>
                <div class="flex-tre">
                    <i class="fa-solid fa-check"></i>
                    <p>We price match to give you the <span>best deals</span></p>
                </div>
            </div>
        </div>

        <!-- ------------------------------------ -->
        <!-- BACKGROUND -->

        <div class="section-background">
            <div class="text-background">
                <p>FIND THE BEST ANIMAL SUPPLIES</p>
                <h2>We know animals are a</h2>
                <h2>part of your family, let us</h2>
                <h2>help take care of them.</h2>
            </div>
            <div class="button-container">
                <button>Learn more about us</button>
            </div>
        </div>

        <!-- ------------------------------------ -->
        <!-- BOTTOM -->

        <div class="intern-section-bottom">
            <figure>
                <img src="../assets/img/03_Get_25_OFF/food-transparent-5.png" alt="">
            </figure>
            <div class="text-off">
                <p>Get $25 OFF your first purchase of our homemade pet food! <span><a href="#">Visit the shop</a></span></p>
            </div>
        </div>

    <!-- ------------------------------------ -->

    </section>

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

.section-uno {

    // ------------------------------------
    // TOP
    
    .intern-section-top {
        background-color: $main-green;
        background-image: url('../assets/img/00_Zampe_background/bg-transparent-3.png');
        background-position: center;
        background-size: 20%;
        width: 864px;
        min-height: 30px;
        // margin: 0 auto;
        font-size: 0.5rem;

        .elements-flex {
            // border: 1px solid red;
            display: flex;
            color: white;
            padding-top: 9px;

            .flex-uno {
                display: flex;
                gap: 5px;
                align-items: center;
            }

            .flex-due {
                display: flex;
                gap: 5px;
                align-items: center;
            }

            .flex-tre {
                display: flex;
                gap: 5px;
                align-items: center;
            }

            span {
                color: white;
            }

            p {
                color: gray;
            }
        }
    }

    // ------------------------------------
    // BACKGROUND

    .section-background {
        background-image: url('../assets/img/02_We_know_animals/banner-5-2x-scaled.jpg');
        background-position: center;
        background-repeat: no-repeat;
        background-size: cover;
        height: 347px;
        width: 864px;
        display: flex;
        flex-direction: column;
        justify-content: center;
        gap: 20px;        

        .text-background {
            color: white;
            // border: 1px solid red;
            margin-left: 120px;
        }

        p {
            font-size: 0.5rem;
            margin-bottom: 15px;
        }

        .button-container {
            // border: 1px solid royalblue;
            margin-left: 120px;
        }

        button {
            border-radius: 10px;
            font-size: 0.5rem;
            padding: 6px 15px;
            border: 0;
            font-weight: 550;
            cursor: pointer;
            display: inline-block;
            vertical-align: middle;
            -webkit-transform: perspective(1px) translateZ(0);
            transform: perspective(1px) translateZ(0);
            box-shadow: 0 0 1px rgba(0, 0, 0, 0);
            -webkit-transition-duration: 0.5s;
            transition-duration: 0.5s;
        }

        button:hover, button:focus, button:active {
            background: $main-green;
            color: white;
            -webkit-transform: scale(1.2);
            transform: scale(1.2);
            -webkit-transition-timing-function: cubic-bezier(0.47, 2.02, 0.31, -0.36);
            transition-timing-function: cubic-bezier(0.47, 2.02, 0.31, -0.36);
        }
    }

    // ------------------------------------
    // BOTTOM

    .intern-section-bottom {
        background-color: $main-green;
        background-image: url('../assets/img/00_Zampe_background/bg-transparent-3.png');
        background-position: center;
        background-size: 20%;
        height: 64px;
        width: 864px;
        position: relative;

        img {
            height: 50px;
            // border: 1px solid red;
            margin-top: 20px;
            margin-left: 50px;
            position: absolute;
            transform: translate( 160%, -12%);
        }

        .text-off {
            // border: 1px solid red;
            display: flex;
            // justify-content: center;
            // align-items: center;
            padding: 25px 0;
            margin-left: 90px;
        }

        p {
            color: white;
            font-size: 0.6rem;
        }

        a {
            color: rgb(223, 223, 223); 
            text-decoration: underline;
            font-size: 0.5rem;
            padding: 0 10px; 
            align-items: center;
        }
    }

    // ------------------------------------

}

</style>

// ------------------------------------