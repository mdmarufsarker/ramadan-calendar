<template>
    <div class="rahmat">
        <h2>10 days of Rahmat</h2>
        <div class="wrapper">
            <div class="parent">
                <span class="title">No.</span>
                <div class="count child" v-for="count in counts" :key="count">
                    {{ count }}
                </div>
            </div>
            <div class="parent">
                <span class="title">Dates</span>
                <div class="dates child" v-for="date in dates" :key="date">
                    {{ date }}
                </div>
            </div>
            <div class="parent">
                <span class="title">Days</span>
                <div class="day child" v-for="day in days" :key="day">
                    {{ day }}
                </div>
            </div>
            <div class="parent">
                <span class="title">Seheri</span>
                <div
                    class="seheri child"
                    v-for="seheri in seheri"
                    :key="seheri"
                >
                    {{ seheri }}
                </div>
            </div>
            <div class="parent">
                <span class="title">Iftar</span>
                <div class="iftar child" v-for="iftar in iftar" :key="iftar">
                    {{ iftar }}
                </div>
            </div>
        </div>
    </div>
</template>

<script>
export default {
    data() {
        return {
            counts: [1, 2, 3, 4, 5, 6, 7, 8, 9, 10],
            dates: [
                "12 March",
                "13 March",
                "14 March",
                "15 March",
                "16 March",
                "17 March",
                "18 March",
                "19 March",
                "20 March",
                "21 March",
            ],
            days: [
                "Tuesday",
                "Wednesday",
                "Thursday",
                "Friday",
                "Saturday",
                "Sunday",
                "Monday",
                "Tuesday",
                "Wednesday",
                "Thursday",
            ],
            seheri: [
                "04:51",
                "04:50",
                "04:49",
                "04:48",
                "04:47",
                "04:46",
                "04:45",
                "04:44",
                "04:43",
                "04:42",
            ],
            iftar: [
                "06:10",
                "06:10",
                "06:11",
                "06:11",
                "06:12",
                "06:12",
                "06:12",
                "06:13",
                "06:13",
                "06:13",
            ],
        };
    },
};
</script>

<style>
.title {
    display: flex;
    justify-content: center;
    padding: 0 10px;
    font-size: 1.4rem;
    font-weight: 600;
    text-decoration: underline;
}
.rahmat {
    width: 500px;
    background-color: cyan;
    margin: 20px;
    border-radius: 10px;
    text-align: center;
    padding: 25px auto;
}
.rahmat h2 {
    font-size: 25px;
    text-align: center;
    padding: 10px 0 5px 0;
    border-bottom: 10px solid dodgerblue;
}
.rahmat .wrapper {
    display: flex;
    flex-direction: row;
    justify-content: space-around;
    padding: 15px;
}
.wrapper .parent {
    line-height: 2;
    font-size: 20px;
}
.wrapper .parent .child {
    padding: 5px 10px;
}

@media (max-width: 1440px) {
    .title {
        font-size: 1.2rem;
    }
    .rahmat {
        width: 400px;
        margin: 15px 10px;
    }

    .rahmat h2 {
        font-size: 20px;
    }

    .wrapper .parent {
        line-height: 1.7;
        font-size: 17px;
    }
}

@media (max-width: 1388px) {
    .title {
        font-size: 1rem;
    }
    .rahmat {
        width: 300px;
        margin: 15px 10px;
    }

    .rahmat h2 {
        font-size: 16px;
    }

    .wrapper .parent {
        line-height: 1.2;
        font-size: 13px;
    }

    .wrapper .parent .child {
        padding: 5px 2px;
    }
}
</style>
