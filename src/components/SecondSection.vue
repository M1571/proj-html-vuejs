// ------------------------------------
// HTML

<template>
    
    <section class="section-due">

        <div class="sec-1">
            <h5>Browse by category</h5>
            <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Voluptatibus voluptatum dolore at possimus.</p>
        </div>
        <div class="sec-2">
            <div v-for="(el,i) in cards" class="card" :key="i">
                <figure>
                    <img :src="el.img" width="150" alt="">
                </figure>
                <div>
                    <p>{{el.text}}</p>
                </div>
            </div>
        </div>
        <div class="sec-3">
            <div class="paw-card">
                <div>
                    <h4>Kibble</h4>
                    <p>Dry dog food</p>
                </div>
                <figure>
                    <img src="../assets/img/05_Kibble_Moist_Frozen/food-transparent-18-400x420.png" width="115" alt="">
                </figure>
                <button>Shop dry food</button>
            </div>
            <div class="paw-card">
                <div>
                    <h4>Moist</h4>
                    <p>Canned dog food</p>
                </div>
                <figure>
                    <img src="../assets/img/05_Kibble_Moist_Frozen/food-transparent-17-400x420.png" width="115" alt="">
                </figure>
                <button>Shop moist food</button>
            </div>
            <div class="paw-card">
                <div>
                    <h4>Frozen</h4>
                    <p>Freeze-Dried dog food</p>
                </div>
                <figure>
                    <img src="../assets/img/05_Kibble_Moist_Frozen/food-transparent-16-400x420.png" width="115" alt="">
                </figure>
                <button>Shop forzen food</button>
            </div>
        </div>
        <div class="sec-4">
            <div class="background-cat">
                <p>FIND THE BEST ANIMAL SUPPLIES</p>
                <h2>New arrivals weekly</h2>
                <button>Learn more about</button>
            </div>
        </div>
        <div class="sec-5"></div>
        <div class="sec-6"></div>

    </section>

</template>

// ------------------------------------
// JS

<script>

export default {
       
  data() {
        return {
            cards: [
                {
                    img: require(`../assets/img/04_Browse_by_category/product-9-600x600.jpg`),
                    text: 'Bed (1)',
                },  
                {
                    img: require(`../assets/img/04_Browse_by_category/product-3-600x600.jpg`),
                    text: 'Food (6)',
                },
                {
                    img: require(`../assets/img/04_Browse_by_category/product-2-600x600.jpg`),
                    text: 'Toys (6)',
                },
                {
                    img: require(`../assets/img/04_Browse_by_category/product-4-600x600.jpg`),
                    text: 'Transport (6)',
                },    
            ]
        }
    }      
       
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
        display: flex;

        .paw-card {
            height: 275px;
            width: 200px;
            background-color: $main-green;
            background-image: url('../assets/img/00_Zampe_background/bg-transparent-3.png');
            background-size: 90%;
            display: flex;
            flex-direction: column;
            justify-content: center;
            gap: 15px;

            h4 {
                color: white;
                text-align: center;
                margin-bottom: 5px;
            }

            p {
                color: #338C51;
                font-size: 0.6rem;
                text-align: center;
            }

            button {
                width: 85px;
                border-radius: 10px;
                font-size: 0.4rem;
                padding: 6px 10px;
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

    .sec-4 {
        border: 1px solid royalblue;
        height: 256px;
        width: 634px;
        display: flex;
        justify-content: center;
        align-items: center;

        .background-cat {
            height: 236px;
            width: 622px;
            background-image: url('../assets/img/06_New_arrivals_weekly/banner-3-2x-scaled.jpg');
            background-position: center;
            background-size: 100%;
            display: flex;
            flex-direction: column;
            justify-content: center;
            gap: 15px;

            button {
                width: 85px;
                border-radius: 10px;
                font-size: 0.4rem;
                padding: 6px 10px;
                border: 0;
                font-weight: 550;
            }

            button:hover {
                background: #3C6F42;
                color: white;
                cursor: pointer;
            }

            h2 {
                color: white;
                font-size: 1.6rem;
            }

            p {
                color: white;
                font-size: 0.4rem;
            }
        }
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