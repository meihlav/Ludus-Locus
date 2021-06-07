<template>
  <main>
    <ReactGlobe />
  </main>
</template>

<script>
import ReactGlobe from "react-globe";

export default {
  name: "Globe",
  components: { ReactGlobe },
};
</script>

<style scoped>
main {
  position: absolute;
  left: 0vw;
  width: 200%;
  height: 100%;
}
main div {
  width: 100%;
  height: 105%;
}
</style>