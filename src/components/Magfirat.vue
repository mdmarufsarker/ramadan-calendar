<template>
  <div class="rahmat">
    <h2>10 days of Magfirat</h2>
    <div class="wrapper">
      <div class="parent">
        <span class="title">Count</span>
        <div class="count child" v-for="count in counts" :key="count">
          {{ count }}
        </div>
      </div>
      <div class="parent">
        <span class="title">Days</span>
        <div class="day child" v-for="day in days" :key="day">{{ day }}</div>
      </div>
      <div class="parent">
        <span class="title">Seheri</span>
        <div class="seheri child" v-for="seheri in seheri" :key="seheri">
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
      days: [
        "Sunday",
        "Monday",
        "Tuesday",
        "Wednesday",
        "Thursday",
        "Friday",
        "Saturday",
        "Sunday",
        "Monday",
        "Tuesday",
      ],
      seheri: [
        "04:28",
        "04:27",
        "04:26",
        "04:25",
        "04:24",
        "04:23",
        "04:22",
        "04:21",
        "04:20",
        "04:19",
      ],
      iftar: [
        "06:18",
        "06:19",
        "06:19",
        "06:20",
        "06:20",
        "06:21",
        "06:21",
        "06:22",
        "06:22",
        "06:22",
      ],
    };
  },
};
</script>

<style></style>
