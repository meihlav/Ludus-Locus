<template>
  <div id="app">
    <HeaderComponent style="width: 100vw; height: 15vh"></HeaderComponent>
    <GlobeComponent style="width: 100vw; height: 100vh"></GlobeComponent>
    <LeftComponent style="width: 100vw; height: 100vh"></LeftComponent>
    <RightComponent style="width: 100vw; height: 100vh"></RightComponent>
    <CardsComponent style="width: 100vw; height: 100vh"></CardsComponent>
    <FooterComponent style="width: 100vw; height: 40vh"></FooterComponent>
  </div>
</template>

<script>
import HeaderComponent from "./components/HeaderComponent";
import GlobeComponent from "./components/GlobeComponent";
import LeftComponent from "./components/LeftComponent";
import RightComponent from "./components/RightComponent";
import CardsComponent from "./components/CardsComponent";
import FooterComponent from "./components/FooterComponent";

export default {
  name: "App",
  components: {
    //Globe,
    HeaderComponent,
    GlobeComponent,
    LeftComponent,
    RightComponent,
    CardsComponent,
    FooterComponent,
  },
  data() {
    return {
      isLoading: true,
    };
  },
  mounted() {
    setTimeout(() => (this.isLoading = false), 3000);
  },
};
</script>

<style>
#app {
  display: flex;
  flex-direction: column;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  padding: 0px;
  margin: -1rem;
  background: #000;

  --size-small: 20px;
  --size-medium: 2vw;
  --size-large: 50px;
}
</style>
