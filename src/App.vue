<template>
  <div>
    <h1>Ramadan Calendar 2023</h1>
    <hr />
    <hr />
    <div class="container">
      <Rahmat />
      <Magfirat />
      <Najat />
    </div>
    <footer>
      <h3>© 2022 Copyright | All rights reserved | Md. Maruf Sarker</h3>
    </footer>
  </div>
</template>

<script>
// import components
import Rahmat from "./components/Rahmat.vue";
import Magfirat from "./components/Magfirat.vue";
import Najat from "./components/Najat.vue";

export default {
  components: {
    Rahmat,
    Magfirat,
    Najat,
  },
  data() {
    return {};
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
  background-color: dodgerblue;
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
</style>
