<template>
  <div class="rahmat">
    <h2>10 days of Rahmat</h2>
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
      counts: [1, 2, 3, 4, 5, 6, 7, 8, 9, 10],
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
        "04:26",
        "04:25",
        "04:24",
        "04:23",
        "04:22",
        "04:21",
        "04:20",
        "04:19",
        "04:18",
        "04:16",
      ],
      iftar: [
        "06:19",
        "06:20",
        "06:20",
        "06:21",
        "06:21",
        "06:22",
        "06:22",
        "06:22",
        "06:23",
        "06:23",
      ],
    };
  },
};
</script>

<style>
.rahmat {
  width: 400px;
  background-color: cyan;
  margin: 20px;
  border-radius: 10px;
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
}
.wrapper .parent {
  line-height: 2;
  font-size: 20px;
}
.wrapper .parent .child {
  padding: 5px 10px;
}
@media only screen and (max-width: 1300px) {
}
</style>
