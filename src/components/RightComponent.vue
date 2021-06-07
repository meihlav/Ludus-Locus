<template>
  <div class="container">
    <div class="texts">
      <div class="titleRight">
        Add Your Place
        <p class="paragraphRight">
          A daily dataset to keep you up to date on<br />subscription market
          trends and what's happening in<br />your vertical.
        </p>
      </div>

      <div class="titleLeft">
        Get Exclusive Content
        <p class="paragraphLeft">
          A daily dataset to keep you up to date on<br />subscription market
          trends and what's happening in<br />your vertical.
        </p>
      </div>

      <div class="titleRight">
        About Infos
        <p class="paragraphRight">
          A daily dataset to keep you up to date on<br />subscription market
          trends and what's happening in<br />your vertical.
        </p>
      </div>
    </div>
    <div class="image"></div>
  </div>
</template>

<script>
export default {
  name: "RightComponent",
  components: {},
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
@import url("https://fonts.googleapis.com/css2?family=Fjord+One&display=swap");

@import url("https://fonts.googleapis.com/css2?family=Mulish:ital,wght@0,200;0,300;0,400;0,500;0,600;0,700;0,800;0,900;1,200;1,300;1,400;1,500;1,600;1,700;1,800;1,900&display=swap");

@import url("https://fonts.googleapis.com/css2?family=DM+Sans:ital,wght@0,400;0,500;0,700;1,400;1,500;1,700&display=swap");
.container {
  display: flex;
  flex-direction: row;
  width: 100vw;
  height: 100vh;
  background: #000;
  padding: 5rem;
}
.image {
  width: 50vw;
  height: 100vh;
  background: url("/second_image.gif");
  background-repeat: no-repeat;
  background-size: 80%;
}
.texts {
  width: 50vw;
  height: 100vh;
  padding-right: 10vw;
}

.Globe {
  z-index: 5;
  width: 100vw;
  height: 100vh;
}

.titleLeft {
  text-align: left;
  font-family: "DM Sans", serif;
  font-style: normal;
  font-weight: bold;
  font-size: var(--size-large);
  line-height: 57px;
  /* identical to box height, or 114% */
  color: #AEAEAE;

  letter-spacing: -1.56316px;
}
.titleRight {
  text-align: right;
  font-family: "DM Sans", serif;
  font-style: normal;
  font-weight: bold;
  font-size: var(--size-large);
  line-height: 57px;
  /* identical to box height, or 114% */
  color: #AEAEAE;

  letter-spacing: -1.56316px;
}

.paragraphLeft {
  text-align: left;
  font-family: "Mulish", serif;
  font-style: normal;
  font-weight: normal;
  font-size: var(--size-small);
  line-height: 30px;
  /* or 150% */

  letter-spacing: -0.625263px;

  color: #696871;
}
.paragraphRight {
  text-align: right;
  font-family: "Mulish", serif;
  font-style: normal;
  font-weight: normal;
  font-size: var(--size-small);
  line-height: 30px;
  /* or 150% */

  letter-spacing: -0.625263px;

  color: #696871;
}
</style>
