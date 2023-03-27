<template>
    <div class="rahmat">
        <h2>10 days of Najat</h2>
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
            counts: [21, 22, 23, 24, 25, 26, 27, 28, 29, 30],
            dates: [
                "13 April",
                "14 April",
                "15 April",
                "16 April",
                "17 April",
                "18 April",
                "19 April",
                "20 April",
                "21 April",
                "22 April",
            ],
            days: [
                "Thursday",
                "Friday",
                "Saturday",
                "Sunday",
                "Monday",
                "Tuesday",
                "Wednesday",
                "Thursday",
                "Friday",
                "Saturday",
              ],
            seheri: [
                "04:16",
                "04:15",
                "04:14",
                "04:13",
                "04:12",
                "04:11",
                "04:10",
                "04:09",
                "04:08",
                "04:07",
            ],
            iftar: [
                "06:23",
                "06:23",
                "06:24",
                "06:24",
                "06:24",
                "06:25",
                "06:25",
                "06:26",
                "06:26",
                "06:27",
            ],
        };
    },
};
</script>

<style></style>
