<template>
  <div class="rahmat">
    <h2>10 days of Najat</h2>
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
      counts: [21, 22, 23, 24, 25, 26, 27, 28, 29, 30],
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
        "04:05",
        "04:05",
        "04:04",
        "04:03",
        "04:02",
        "04:01",
        "04:00",
        "03:59",
        "03:58",
        "03:59",
      ],
      iftar: [
        "06:18",
        "06:28",
        "06:29",
        "06:29",
        "06:29",
        "06:30",
        "06:30",
        "06:31",
        "06:31",
        "06:32",
      ],
    };
  },
};
</script>

<style></style>
