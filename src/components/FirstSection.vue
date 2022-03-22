// ------------------------------------
// HTML

<template>

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
        
    </div>

    <!-- ------------------------------------ -->
    <!-- BOTTOM -->

    <!-- <div class="intern-section-bottom">

    </div> -->

    <!-- ------------------------------------ -->

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

.intern-section-top {
    background-color: $main-green;
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
    }

    span {
        color: white;
    }

    p {
        color: gray;
    }
}

</style>

// ------------------------------------