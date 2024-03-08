<template>
    <div class="rahmat">
        <h2>10 days of Magfirat</h2>
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
            counts: [11, 12, 13, 14, 15, 16, 17, 18, 19, 20],
            dates: [
                "22 March",
                "23 March",
                "24 March",
                "25 March",
                "26 March",
                "27 March",
                "28 March",
                "29 March",
                "30 March",
                "31 March",
            ],
            days: [
                "Friday",
                "Saturday",
                "Sunday",
                "Monday",
                "Tuesday",
                "Wednesday",
                "Thursday",
                "Friday",
                "Saturday",
                "Sunday",
            ],
            seheri: [
                "04:41",
                "04:40",
                "04:39",
                "04:38",
                "04:36",
                "04:35",
                "04:34",
                "04:33",
                "04:31",
                "04:30",
            ],
            iftar: [
                "06:14",
                "06:14",
                "06:14",
                "06:15",
                "06:15",
                "06:16",
                "06:16",
                "06:17",
                "06:17",
                "06:18",
            ],
        };
    },
};
</script>

<style></style>
