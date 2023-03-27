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
                "03 April",
                "04 April",
                "05 April",
                "06 April",
                "07 April",
                "08 April",
                "09 April",
                "10 April",
                "11 April",
                "12 April",
            ],
            days: [
                "Monday",
                "Tuesday",
                "Wednesday",
                "Thursday",
                "Friday",
                "Saturday",
                "Sunday",
                "Monday",
                "Tuesday",
                "Wednesday",
            ],
            seheri: [
                "04:27",
                "04:26",
                "04:25",
                "04:24",
                "04:23",
                "04:22",
                "04:21",
                "04:20",
                "04:19",
                "04:18",
            ],
            iftar: [
                "06:19",
                "06:19",
                "06:20",
                "06:20",
                "06:21",
                "06:21",
                "06:22",
                "06:22",
                "06:22",
                "06:23",
            ],
        };
    },
};
</script>

<style></style>
