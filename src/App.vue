<template>
    <!--<div>-->
    <!--    <h1>Ramadan Calendar {{ year }}</h1>-->
    <!--    <hr />-->
    <!--    <hr />-->
    <!--    <div class="container">-->
    <!--        <Rahmat />-->
    <!--        <Magfirat />-->
    <!--        <Najat />-->
    <!--    </div>-->
    <!--    <footer>-->
    <!--        <h3>© {{ year }} Contributed by - Md. Maruf Sarker & Saadman Galib</h3>-->
    <!--    </footer>-->
    <!--</div>-->

        <ComingSoon/>
</template>

<script>
// import components
//import Rahmat from "./components/Rahmat.vue";
//import Magfirat from "./components/Magfirat.vue";
//import Najat from "./components/Najat.vue";
//
//const year = new Date().getFullYear();

import ComingSoon from "./pages/ComingSoon/ComingSoon.vue";

export default {
    components: {
//        Rahmat,
//        Magfirat,
//        Najat,
        ComingSoon
    },
    data() {
        return {
//            year,
        };
    },
};
</script>

<style>
@import url("https://fonts.googleapis.com/css2?family=Itim&display=swap");

* {
    margin: 0;
    padding: 0;
    box-sizing: border-box;
}

body {
    font-family: "Itim", cursive;
    /*    background-color: dodgerblue;*/
}

h1 {
    color: #fff;
    text-align: center;
    padding-top: 20px;
}

hr {
    height: 2px;
    width: 300px;
    margin: 3px auto;
    background-color: #000;
    border: none;
}

.main-container{
    min-height: 100vh;
    width: 60%;
    margin: auto;
}

.container {
    display: flex;
    flex-direction: row;
    margin-top: 10px;
    justify-content: space-around;
    flex-wrap: wrap;
}

h3 {
    text-align: center;
    font-weight: 400;
    margin-bottom: 10px;
}

@media (min-width: 1921px) {
    #app {
        width: 1920px;
        margin-left: auto;
        margin-right: auto;
    }
}

@media (max-width: 1440px) {
    .container {
        width: 80%;
        margin: auto;
    }

    footer {
        font-size: 10px;
        width: 80%;
        margin: auto;
    }
}

@media (max-width: 1024px) {
    .container {
        width: 90%;
        margin: auto;
    }

    h1 {
        font-size: 28px;
    }

    hr {
        height: 1.3px;
        width: 90%;
    }
}
</style>
