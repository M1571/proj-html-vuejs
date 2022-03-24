// ------------------------------------
// HTML

<template>
    
    <section class="section-due">

        <div class="sec-1">
            <h5>Browse by category</h5>
            <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Voluptatibus voluptatum dolore at possimus.</p>
        </div>
        <div class="sec-2">
            <div class="card">
                <figure>
                    <img src="../assets/img/04_Browse_by_category/product-9-600x600.jpg" width="150" alt="">
                </figure>
                <div>
                    <p>Bed (1)</p>
                </div>
            </div>
            <div class="card">
                <figure>
                    <img src="../assets/img/04_Browse_by_category/product-3-600x600.jpg" width="150" alt="">
                </figure>
                <div>
                    <p>Food (6)</p>
                </div>
            </div>
            <div class="card">
                <figure>
                    <img src="../assets/img/04_Browse_by_category/product-2-600x600.jpg" width="150" alt="">
                </figure>
                <div>
                    <p>Toys (6)</p>
                </div>
            </div>
            <div class="card">
                <figure>
                    <img src="../assets/img/04_Browse_by_category/product-4-600x600.jpg" width="150" alt="">
                </figure>
                <div>
                    <p>Transport (6)</p>
                </div>
            </div>
        </div>
        <div class="sec-3"></div>
        <div class="sec-4"></div>
        <div class="sec-5"></div>
        <div class="sec-6"></div>

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

.section-due {
    border: 1px solid green;
    width: 864px;
    height: 1275px;
    display: flex;
    flex-direction: column;
    gap: 30px;
    padding: 60px;

    .sec-1 {
        border: 1px solid royalblue;
        height: 61px;
        width: 315px;
        text-align: center;

        h5 {
            font-size: 1rem;
        }

        p {
            font-size: 0.7rem;
            margin-top: 10px;
        }
    }

    .sec-2 {
        border: 1px solid royalblue;
        height: 194px;
        width: 634px;
        display: flex;

        .card {

            p {
                text-align: center;
                font-size: 0.8rem;
            }
        }

    }

    .sec-3 {
        border: 1px solid royalblue;
        height: 295px;
        width: 634px;
    }

    .sec-4 {
        border: 1px solid royalblue;
        height: 256px;
        width: 634px;
    }

    .sec-5 {
        border: 1px solid royalblue;
        height: 58px;
        width: 634px;
    }

    .sec-6 {
        border: 1px solid royalblue;
        height: 194px;
        width: 634px;
    }
}

</style>

// ------------------------------------