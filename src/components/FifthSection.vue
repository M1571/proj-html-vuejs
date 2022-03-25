// ------------------------------------
// HTML

<template>
    
    <section class="section-cinque">
        <div class="title-cards">
            <h2>New products arrival</h2>
            <p>Latest products</p>
        </div>
        <div class="container-cards">
            <div class="card">
                <figure>
                    <img src="../assets/img/13_New_products_arrival/product-8-600x600.jpg" width="200" alt="">
                </figure>
                <div>
                    <h5>Colored pet bed</h5>
                    <p>$18.00 - $26.00</p>
                </div>
            </div>
            <div class="card">
                <figure>
                    <img src="../assets/img/13_New_products_arrival/product-2-600x600.jpg" width="200" alt="">
                </figure>
                <div>
                    <h5>Colorful ball set</h5>
                    <p>$29.00</p>
                </div>
            </div>
            <div class="card">
                <figure>
                    <img src="../assets/img/13_New_products_arrival/product-3-600x600.jpg" width="200" alt="">
                </figure>
                <div>
                    <h5>Dog bone</h5>
                    <p>$18.00</p>
                </div>
            </div>
            <div class="card">
                <figure>
                    <img src="../assets/img/13_New_products_arrival/product-4-600x600.jpg" width="200" alt="">
                </figure>
                <div>
                    <h5>Animal transport bag</h5>
                    <p>$29.00</p>
                </div>
            </div>
            <div class="card">
                <figure>
                    <img src="../assets/img/13_New_products_arrival/product-5-600x600.jpg" width="200" alt="">
                </figure>
                <div>
                    <h5>Animal transport cage</h5>
                    <p>$35.00</p>
                </div>
            </div>
            <div class="card">
                <figure>
                    <img src="../assets/img/13_New_products_arrival/product-10-600x600.jpg" width="200" alt="">
                </figure>
                <div>
                    <h5>Closable cat litter</h5>
                    <p>$16.00</p>
                </div>
            </div>
        </div>
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

.section-cinque {
    // border: 1px solid green;
    width: 864px;
    height: 684px;
    display: flex;
    flex-direction: column;
    justify-content: center;
    gap: 30px;

    .title-cards {
        // border: 1px solid blue;
        text-align: center;
        
        h2 {
            color: $titolone-color;
            font-size: 1rem;
            margin-bottom: 5px;
        }

        p {
            color: #3C6F42;
            font-size: 0.6rem;
        }
    }

    .container-cards {
        // border: 1px solid red;
        text-align: center;
        width: 629px;
        height: 512px;
        display: flex;
        flex-wrap: wrap;
        
        .card {
            display: flex;
            flex-direction: column;
            display: inline-block;
            vertical-align: middle;
            -webkit-transform: perspective(1px) translateZ(0);
            transform: perspective(1px) translateZ(0);
            box-shadow: 0 0 1px rgba(0, 0, 0, 0);
            -webkit-transition-duration: 0.3s;
            transition-duration: 0.3s;
            -webkit-transition-property: transform;
            transition-property: transform;
            
            img {
                cursor: pointer;
            }

            h5 {
                margin-bottom: 5px;
            }

            p {
                color: #3C6F42;
                font-size: 0.6rem;
            }
        }

        .card:hover, .card:focus, .card:active {
            -webkit-transform: scale(1.1);
            transform: scale(1.1);
        }
    }
}

</style>

// ------------------------------------