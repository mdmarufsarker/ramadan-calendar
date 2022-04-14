<template>
  <div class="rahmat">
    <h2>10 days of Magfirat</h2>
    <div class="wrapper">
      <div class="parent">
        <div class="count child" v-for="count in counts" :key="count">
          {{ count }}
        </div>
      </div>
      <div class="parent">
        <div class="day child" v-for="day in days" :key="day">{{ day }}</div>
      </div>
      <div class="parent">
        <div class="seheri child" v-for="seheri in seheri" :key="seheri">
          {{ seheri }}
        </div>
      </div>
      <div class="parent">
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
        "04:15",
        "04:14",
        "04:13",
        "04:12",
        "04:11",
        "04:10",
        "04:09",
        "04:08",
        "04:07",
        "04:06",
      ],
      iftar: [
        "06:23",
        "06:24",
        "06:24",
        "06:24",
        "06:25",
        "06:25",
        "06:26",
        "06:26",
        "06:27",
        "06:27",
      ],
    };
  },
};
</script>

<style></style>
