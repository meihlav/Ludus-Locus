<template>
  <div class="container">
    <div class="column">
      <div class="firstRow">
        <div class="footerText">
          Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do
          eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad
          minim veniam, quis nostrud exercitation ullamco laboris nisi ut
          aliquip ex ea commodo consequat.
        </div>
        <div>
          <h1 class="inputLabel">Subscribe to our newsletter</h1>
          <div class="inputContainer">
            <input placeholder="Email address" class="input" />
            <div class="inputButton"><p>></p></div>
          </div>
        </div>
        <div>
          <p class="title">Services</p>
          <p class="paragraph">3D Models</p>
          <p class="paragraph">Campaigns</p>
          <p class="paragraph">Branding</p>
        </div>
        <div>
          <p class="title">Follow Us</p>
          <p class="paragraph">Facebook</p>
          <p class="paragraph">Instagram</p>
        </div>
      </div>
      <div
        class="secondRow"
        style="display: flex; justify-content: center; gap: 1rem"
      >
        <p class="paragraph">Terms & Conditions</p>
        <p class="paragraph">Privacy Policy</p>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "FooterComponent",
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
.container {
  padding-top: 2rem;
  width: 100%;
  height: 40%;
  background: #000;
  display: flex;
  justify-content: center;
}

.firstRow {
  display: flex;
  justify-content: space-between;
  text-align: left;
  width: 1092px;
  height: 124px;
}

.footerText {
  height: 120px;
  width: 293px;

  font-family: "DM Sans", serif;
  font-style: normal;
  font-weight: normal;
  font-size: 15px;
  line-height: 20px;
  letter-spacing: -0.204545px;

  color: #FFFFFF;
}

.inputContainer {
  display: flex;
}

.inputLabel {
  height: 58px;
  width: 165px;
  font-family: "DM Sans", serif;
  font-style: normal;
  font-weight: normal;
  font-size: 22px;
  line-height: 29px;
  letter-spacing: -0.3px;

  color: #FFFFFF;
}

.input {
  background: rgba(0, 0, 0, 0);
  border: none;
  border-bottom: 1px solid rgba(255, 255, 255, 0.1);
}

.inputButton {
  display: flex;
  justify-content: center;
  width: 50px;
  height: 50px;
  background: #272764;
  color: #fff;
  border-radius: 10px 10px 0px 0px;
}
.title {
  height: 22px;

  font-family: "DM Sans", serif;
  font-style: normal;
  font-weight: normal;
  font-size: 17px;
  line-height: 22px;
  letter-spacing: -0.231818px;

  /* Primary */

  color: #5454D4;
}
.paragraph {
  height: 20px;
  left: 69.86%;
  right: 24.79%;
  top: calc(50% - 20px / 2 - 7px);

  font-family: "DM Sans", serif;
  font-style: normal;
  font-weight: normal;
  font-size: 15px;
  line-height: 20px;
  /* identical to box height */

  letter-spacing: -0.204545px;

  color: #FFFFFF;
}

.secondRow {
  padding: 2rem;
}
</style>
