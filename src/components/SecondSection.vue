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
        <div class="sec-5">
            <div>
                <p>All-time best seller</p>
                <h4>Items everyone loves</h4>
            </div>
            <div>
                <button>View all products</button>
            </div>
        </div>
        <div class="sec-6">
            <div v-for="(el,i) in smcards" class="smcards" :key="i">
                <figure>
                    <img :src="el.img" width="140" alt="">
                </figure>
                <div>
                    <h4>{{el.texth}}</h4>
                    <p>{{el.textp}}</p>
                </div>
            </div>
        </div>

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
            ],
            smcards: [
                {
                    img: require(`../assets/img/07_Items_everyone_loves/product-21-400x400.jpg`),
                    texth: 'Transport cage',
                    textp: '$25.00',
                },
                {
                    img: require(`../assets/img/07_Items_everyone_loves/product-20-400x400.jpg`),
                    texth: 'Dog leash',
                    textp: '$25.00',
                },
                {
                    img: require(`../assets/img/07_Items_everyone_loves/product-16-400x400.jpg`),
                    texth: 'Animal transport cage',
                    textp: '$25.00',
                },
                {
                    img: require(`../assets/img/07_Items_everyone_loves/product-11-400x400.jpg`),
                    texth: 'Colorful cat leash',
                    textp: '$12.00',
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
    // border: 1px solid $main-green;
    width: 864px;
    height: 1275px;
    display: flex;
    flex-direction: column;
    gap: 30px;
    padding: 60px;

    .sec-1 {
        // border: 1px solid royalblue;
        height: 61px;
        width: 315px;
        text-align: center;

        h5 {
            font-size: 1rem;
            color: #1E4346;
        }

        p {
            font-size: 0.7rem;
            margin-top: 10px;
            color: #1E4346;
        }
    }

    .sec-2 {
        // border: 1px solid royalblue;
        height: 194px;
        width: 634px;
        display: flex;

        .card {

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

            p {
                text-align: center;
                font-size: 0.8rem;
            }
        }

        .card:hover, .card:focus, .card:active {
            -webkit-transform: scale(1.1);
            transform: scale(1.1);
        }

    }

    .sec-3 {
        // border: 1px solid royalblue;
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
                display: inline-block;
                vertical-align: middle;
                -webkit-transform: perspective(1px) translateZ(0);
                transform: perspective(1px) translateZ(0);
                box-shadow: 0 0 1px rgba(0, 0, 0, 0);
                -webkit-transition-duration: 0.5s;
                transition-duration: 0.5s;
            }

            button:hover, button:focus, button:active {
                background: #3C6F42;
                color: white;
                cursor: pointer;
                -webkit-transform: scale(1.2);
                transform: scale(1.2);
                -webkit-transition-timing-function: cubic-bezier(0.47, 2.02, 0.31, -0.36);
                transition-timing-function: cubic-bezier(0.47, 2.02, 0.31, -0.36);
            }
        }
    }

    .sec-4 {
        // border: 1px solid royalblue;
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
                display: inline-block;
                vertical-align: middle;
                -webkit-transform: perspective(1px) translateZ(0);
                transform: perspective(1px) translateZ(0);
                box-shadow: 0 0 1px rgba(0, 0, 0, 0);
                -webkit-transition-duration: 0.5s;
                transition-duration: 0.5s;
            }

            button:hover, button:focus, button:active {
                background: #3C6F42;
                color: white;
                cursor: pointer;
                -webkit-transform: scale(1.2);
                transform: scale(1.2);
                -webkit-transition-timing-function: cubic-bezier(0.47, 2.02, 0.31, -0.36);
                transition-timing-function: cubic-bezier(0.47, 2.02, 0.31, -0.36);
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
        // border: 1px solid royalblue;
        height: 58px;
        width: 634px;
        display: flex;
        justify-content: space-between;
        align-items: center;
        gap: 350px;

        button {
                width: 85px;
                border-radius: 10px;
                font-size: 0.4rem;
                padding: 6px 10px;
                border: 0;
                font-weight: 550;
                display: inline-block;
                vertical-align: middle;
                -webkit-transform: perspective(1px) translateZ(0);
                transform: perspective(1px) translateZ(0);
                box-shadow: 0 0 1px rgba(0, 0, 0, 0);
                -webkit-transition-duration: 0.5s;
                transition-duration: 0.5s;
            }

            button:hover, button:focus, button:active {
                background: #3C6F42;
                color: white;
                cursor: pointer;
                -webkit-transform: scale(1.2);
                transform: scale(1.2);
                -webkit-transition-timing-function: cubic-bezier(0.47, 2.02, 0.31, -0.36);
                transition-timing-function: cubic-bezier(0.47, 2.02, 0.31, -0.36);
            }

            h4 {
                color: #1E4346;
                font-size: 1.1rem;
                margin-top: 5px;
            }

            p {
                color: #1E4346;
                font-size: 0.6rem;
            }
    }

    .sec-6 {
        // border: 1px solid royalblue;
        height: 194px;
        width: 634px;
        display: flex;

        .smcards {

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

            h4 {
                color: #1E4346;
                text-align: center;
                font-size: 0.7rem;
                margin-bottom: 3px;
                margin-top: 3px;
            }

            p {
                color: #338C51;
                text-align: center;
                font-size: 0.6rem;
            }
        }

        .smcards:hover, .smcards:focus, .smcards:active {
            -webkit-transform: scale(1.1);
            transform: scale(1.2);
        }
    }
}

</style>

// ------------------------------------