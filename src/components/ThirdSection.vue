// ------------------------------------
// HTML

<template>
    
    <section class="section-tre">
        <h3>Users testimonials</h3>
        <div class="card-cont">
            <div class="test-card">
                <img src="../assets/img/08_Users_testimonials/avatar-3-200x200.jpg" width="45" alt="">
                <p>Lorem ipsum dolor sit amet, consectetur adipisicing elit. Illum, laboriosam?</p>
                <p class="gray">Lisa Smith, ThemeFusion</p>
            </div>
            <div class="test-card">
                <img src="../assets/img/08_Users_testimonials/avatar-1-200x200.jpg" width="45" alt="">
                <p>Lorem ipsum dolor sit amet, consectetur adipisicing elit. Illum, laboriosam?</p>
                <p class="gray">Melissa Green, ThemeFusion</p>
            </div>
            <div class="test-card">
                <img src="../assets/img/08_Users_testimonials/avatar-4-200x200.jpg" width="45" alt="">
                <p>Lorem ipsum dolor sit amet, consectetur adipisicing elit. Illum, laboriosam?</p>
                <p class="gray">Sam Lewis, ThemeFusion</p>
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

.section-tre {
    background-color: $main-green;
    background-image: url('../assets/img/00_Zampe_background/bg-transparent-3.png');
    background-size: 20%;
    width: 864px;
    height: 310px;
    display: flex;
    flex-direction: column;
    justify-content: center;
    gap: 30px;

    h3 {
        color: white;
    }

    .card-cont {
        display: flex;
        gap: 40px;
    }

    .test-card{
        color: white;
        width: 165px;
        height: 140px;
        // border: 1px solid red;
        display: flex;
        flex-direction: column;
        text-align: center;
        font-size: 0.5rem;
        gap: 10px;

        .gray {
            color: gray;
        }

        img {
            border-radius: 9999px;
        }
    }
}

</style>

// ------------------------------------