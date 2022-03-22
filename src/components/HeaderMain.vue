// ------------------------------------
// HTML

<template>
    
    <header>

        <!-- ------------------------------------ -->
        <!-- HEADER TOP -->

        <div class="header-top">
            <div class="container_header-top">

                <figure>
                    <img src="../assets/img/01_Avada_Pet_Supplies/dark-pet-logo-2x.png" alt="logo-pet-supplies">
                </figure>

                <input type="search" name="" id="">

                <p>Questions?<span> Call us : 1.800.123.4567</span></p>

                <ul>
                    <li>
                        Icona1<i class="fa-regular fa-bag-shopping"></i>
                    </li>
                    <li>
                        Icona2<i class="fa-regular fa-user"></i>
                    </li>
                </ul>

            </div>
        </div>

        <!-- ------------------------------------ -->
        <!-- HEADER BOTTOM -->

        <div class="header-bottom">
            <div class="container_header-bottom">

                <nav class="header-nav">
                    <ul>
                        <li v-for="(link,i) in links" :key="i" class="nav-item" :class="link.active ? 'active' : '' ">
                            <a href="#">{{ link.text }}</a>
                        </li>
                    </ul>
                </nav>

            </div>
        </div>

        <!-- ------------------------------------ -->

    </header>

</template>

// ------------------------------------
// JS

<script>

export default {
       
    data() {
        return {
            links: [
                {
                    text: 'Home',
                    href: '#',
                    // active: true,
                },
                {
                    text: 'Shop',
                    href: '#',         
                },
                {
                    text: 'About',
                    href: '#'
                },
                {
                    text: 'Blog',
                    href: '#'
                },
                {
                    text: 'Contact',
                    href: '#'
                },
                {
                    text: 'Shop by brand',
                    href: '#'
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

header {
    font-size: 0.6rem;
}

// ------------------------------------
// HEADER TOP

.header-top {
    // border: 3px solid royalblue;
    width: 864px;
    min-height: 33px;
    margin: 0 auto;
    display: flex;
    justify-content: center;

    .container_header-top {
        display: flex;
        justify-content: space-evenly;
        // border: 1px solid red;
        align-self: center;
        width: 100%;

        img {
            width: 108px;
        }

        input {
            width: 166px;
            height: 20px;
            border-radius: 9px;       
        }

        span {
            color: #A2A2A2;
        }

        p {
            align-self: center;
        }

        ul {
            display: flex;
            gap: 7px;
            align-self: center;
        }
    }
}

// ------------------------------------
// HEADER BOTTOM

.header-bottom {
    // border: 3px solid salmon;
    border-top: 1px solid lightgray;
    width: 864px;
    min-height: 29px;
    margin: 0 auto;
    display: flex;
    justify-content: center;
    // align-content: center;

    .container_header-bottom {
        // border: 1px solid yellow;
        align-self: center;

        .header-nav {
            display: flex;
            gap: 30px;
            // justify-content: center;

            ul {
                display: contents;
                color: #A2A2A2;
                
            }

            ul:hover {
                color: black;
            }
        }
    }
}

// ------------------------------------

</style>

// ------------------------------------