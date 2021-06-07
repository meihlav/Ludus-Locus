<template>
  <div class="container" style="display: flex; justify-content: space-around">
    <div class="leftSide" style="display: flex; align-items: center">
      <img src="../assets/luduslogo.png" style="width: 10vh" />
      <h1>Ludus Locus</h1>
    </div>
    <div
      class="rightSide"
      style="display: flex; gap: 5rem; align-items: center"
    >
      <p>Home</p>
      <p>Contents</p>
      <p>Services</p>
      <p>Prices</p>
    </div>
  </div>
</template>

<script>
export default {
  name: "HeaderComponent",
  data() {
    return {};
  },
  methods: {},
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
@import url("https://fonts.googleapis.com/css2?family=Fjord+One&display=swap");

@import url("https://fonts.googleapis.com/css2?family=Mulish:ital,wght@0,200;0,300;0,400;0,500;0,600;0,700;0,800;0,900;1,200;1,300;1,400;1,500;1,600;1,700;1,800;1,900&display=swap");

@import url("https://fonts.googleapis.com/css2?family=DM+Sans:ital,wght@0,400;0,500;0,700;1,400;1,500;1,700&display=swap");

@import url("https://fonts.googleapis.com/css2?family=IBM+Plex+Mono:wght@200;300;400;500;600;700&display=swap");

.container {
  width: 100%;
  height: 15vh;
  background: #000;
}

h1 {
  font-family: "IBM Plex Mono";
  font-style: normal;
  font-weight: normal;
  font-size: 36px;
  line-height: 47px;
  display: flex;
  align-items: flex-end;

  color: #FFFFFF;
}
p {
  font-family: "DM Sans", serif;
  font-style: normal;
  font-weight: bold;
  font-size: 15px;
  line-height: 20px;
  /* identical to box height */

  letter-spacing: -0.468947px;

  color: #696871;
}
p:hover {
  color: #fff;
  border-bottom: 1px solid #5454D4;
}
</style>
