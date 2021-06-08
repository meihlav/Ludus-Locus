<template>
  <div class="container">
    <div class="Info">
      <h1>
        Discover playable<br />
        places & events 🗺
      </h1>
      <p class="paragraph">
        We provide for free more than 10,000 places in a interactive map to see
        the<br />easiest way to find the best places across the world to have a
        Good Game :)
      </p>
      <button class="StartedButton">
        <p class="StartedButtonInfo">Get Started</p>
      </button>
    </div>
    <div class="Globe">
      <a href="https://ludus-locus-map.vercel.app/">
        <Globe></Globe>
      </a>
    </div>
  </div>
</template>

<script>
import Globe from "./Globe";
export default {
  name: "GlobeComponent",
  components: {
    Globe,
  },
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
@import url("https://fonts.googleapis.com/css2?family=Fjord+One&display=swap");

@import url("https://fonts.googleapis.com/css2?family=Mulish:ital,wght@0,200;0,300;0,400;0,500;0,600;0,700;0,800;0,900;1,200;1,300;1,400;1,500;1,600;1,700;1,800;1,900&display=swap");

@import url("https://fonts.googleapis.com/css2?family=DM+Sans:ital,wght@0,400;0,500;0,700;1,400;1,500;1,700&display=swap");

@keyframes inEffect {
  from {
    opacity: 0;
  }
  to {
    opacity: 1;
  }
}
.container {
  animation: inEffect 5s;
  width: 100%;
  height: 100%;
}

.Info {
  display: flex;
  flex-direction: column;
  justify-content: left;
  padding: 1rem;
  z-index: 5;
  width: 65vw;
  height: 100vh;
  position: absolute;
  /* background: linear-gradient(
    90deg,
    rgba(0, 0, 0, 1) 80%,
    rgba(0, 0, 0, 0) 100%
  );*/
}

.Globe {
  z-index: 5;
  width: 100vw;
  height: 100vh;
}

h1 {
  margin: 10rem 1rem 1rem 1rem;
  font-family: "Fjord One", serif;
  font-style: normal;
  font-weight: normal;
  font-size: 80px;
  line-height: 77px;
  color: #AEAEAE;
}
.paragraph {
  font-family: "Mulish", serif;
  font-style: normal;
  font-weight: normal;
  font-size: 20px;
  line-height: 30px;
  /* or 150% */

  letter-spacing: -0.625263px;

  color: #696871;
}
.StartedButton {
  background: #5454D4;
  margin-left: 10vw;
  width: 250px;
  height: 64px;
  border-radius: 10px;
  border: none;
}

.StartedButtonInfo {
  font-family: "DM Sans", serif;
  font-style: normal;
  font-weight: bold;
  font-size: 17px;
  line-height: 22px;
  text-align: center;
  letter-spacing: -0.531474px;
  color: #fff;
}
</style>
