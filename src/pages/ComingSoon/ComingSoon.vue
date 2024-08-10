<script setup>
import { ref } from "vue";

const month = ref(0);
const day = ref(0);
const hour = ref(0);
const minute = ref(0);
const second = ref(0);

setInterval(() => {
    const comingSoonDate = new Date("2025-02-28");
    const currentDate = new Date();

    const totalSeconds = (comingSoonDate - currentDate) / 1000;
    const days = Math.floor(totalSeconds / 60 / 60 / 24);
    const months = Math.floor(days / 30);
    const remainingDays = days % 30;
    const hours = Math.floor(totalSeconds / 60 / 60) % 24;
    const minutes = Math.floor(totalSeconds / 60) % 60;
    const seconds = Math.floor(totalSeconds) % 60;

    month.value = months;
    day.value = remainingDays;
    hour.value = hours;
    minute.value = minutes;
    second.value = seconds;
}, 1000);
</script>

<template>
    <div class="coming-soon-page-container">
        <div class="main-container">
            <!-- <div class="coming-soon-nav">
                <div class="nav-left-part"><p>Ramadan Calendar</p></div>
            </div> -->
            <div class="coming-soon-hero-section-container">
                <div class="hero-text-container">
                    <h2>Ramadan 2025</h2>
                    <p>
                        Assalam o alaikum, dear muslims! how are you? ramadan is
                        coming again in
                    </p>
                </div>
                <div class="coming-soon-time-container">
                    <div class="coming-soon-time">
                        <h2>{{ month }}</h2>
                        <p>Months</p>
                    </div>

                    <div class="coming-soon-time">
                        <h2>{{ day }}</h2>
                        <p>Days</p>
                    </div>
                    <div class="coming-soon-time">
                        <h2>{{ hour }}</h2>
                        <p>hours</p>
                    </div>
                    <div class="coming-soon-time">
                        <h2>{{ minute }}</h2>
                        <p>minutes</p>
                    </div>
                    <div class="coming-soon-time">
                        <h2>{{ second }}</h2>
                        <p>seconds</p>
                    </div>
                </div>
            </div>
        </div>
    </div>
</template>

<style scoped>
@import url("https://fonts.googleapis.com/css2?family=Darker+Grotesque:wght@300..900&display=swap");

.coming-soon-page-container {
    min-height: 100vh;
    min-width: 100%;
    background: url("/ramadan-coming-soon-bg.jpg") center/cover #154130;
    font-family: "Darker Grotesque", sans-serif;
}

.coming-soon-nav {
    padding: 30px 0%;
}

.coming-soon-hero-section-container{
    height: 100vh;
    display: flex;
    flex-direction: column;
    align-items: center;
    justify-content: center;
}

.coming-soon-hero-section-container .hero-text-container h2 {
    font-size: 100px;
    color: #fff;
    text-align: center;
}

.coming-soon-hero-section-container .hero-text-container p {
    font-size: 50px;
    color: #fff;
    text-align: center;
    margin: 20px auto 40px auto;
    width: 90%;

}

.coming-soon-time-container {
    display: flex;
    flex-direction: row;
    align-items: center;
    justify-content: center;
    color: #fff;
}

.coming-soon-time {
    margin: 0 20px;
    display: flex;
    flex-direction: column;
    align-items: center;
    width: 120px;
}

.coming-soon-time h2 {
    font-size: 100px;
}

.coming-soon-time p {
    font-size: 30px;
}
</style>
