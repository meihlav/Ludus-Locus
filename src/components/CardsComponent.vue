<template>
  <div class="container">
    <div>
      <div
        style="
          gap: 5rem;
          display: flex;
          justify-content: center;
          align-items: center;
        "
      >
        <h1 class="title">Get the right plan<br />for your business.</h1>

        <div v-on:click="changePrice">
          <div
            v-if="this.Plano === true"
            style="display: flex; flex-direction: row"
          >
            <div class="anualDeactive">Yearly</div>

            <div class="mensalActive">Monthly</div>
          </div>

          <div v-else style="display: flex; flex-direction: row">
            <div class="anualActive">Yearly</div>

            <div class="mensalDeactive">Monthly</div>
          </div>
        </div>
      </div>
      <div
        style="
          display: flex;
          flex-direction: row;
          align-items: flex-end;
          gap: 1rem;
        "
      >
        <div class="firstCard" style="border-radius: 10px">
          <p class="cardTitle">Starter</p>
          <h1 class="price">Free</h1>
          <p class="paragraph">1 Website</p>
          <p class="paragraph">5 GB Hosting</p>
          <p class="paragraph">Limited Support</p>

          <button class="StartedButton">
            <p class="StartedButtonInfo">Get Started</p>
          </button>
        </div>

        <div class="secondCard" style="border-radius: 10px">
          <p class="cardTitle" style="color: #fff">Premium</p>
          <div
            class="price"
            style="
              display: flex;
              flex-direction: row;
              justify-content: center;
              align-items: center;
            "
          >
            ${{ PremiumPrice }}
            <p class="plano">/{{ ThisPlano }}</p>
          </div>
          <p class="paragraph" style="color: #fff">10 Website</p>
          <p class="paragraph" style="color: #fff">15 GB Hosting</p>
          <p class="paragraph" style="color: #fff">Premium Support</p>

          <button class="StartedButton">
            <p class="StartedButtonInfo">Get Started</p>
          </button>
        </div>

        <div class="thirdCard" style="border-radius: 10px">
          <p class="cardTitle" style="color: #fff">Enterprise</p>
          <div
            class="price"
            style="
              display: flex;
              flex-direction: row;
              justify-content: center;
              align-items: center;
            "
          >
            ${{ EnterprisePrice }}
            <p class="plano">/{{ ThisPlano }}</p>
          </div>
          <p class="paragraph" style="color: #fff">Unlimited Website</p>
          <p class="paragraph" style="color: #fff">50 GB Hosting</p>
          <p class="paragraph" style="color: #fff">Ilimited Support</p>

          <button class="StartedButton">
            <p class="StartedButtonInfo">Get Started</p>
          </button>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "CardsComponent",
  data() {
    return {
      Plano: true,
      ThisPlano: "month",
      PremiumPrice: 29,
      EnterprisePrice: 49,
    };
  },
  methods: {
    changePrice() {
      if (this.Plano === false) {
        this.Plano = true;
        this.PremiumPrice = 29;
        this.EnterprisePrice = 49;
        this.ThisPlano = "month";
      } else {
        this.Plano = false;
        this.PremiumPrice = this.PremiumPrice * 12;
        this.EnterprisePrice = this.EnterprisePrice * 12;
        this.ThisPlano = "year";
      }
    },
  },
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
@import url("https://fonts.googleapis.com/css2?family=Fjord+One&display=swap");

@import url("https://fonts.googleapis.com/css2?family=Mulish:ital,wght@0,200;0,300;0,400;0,500;0,600;0,700;0,800;0,900;1,200;1,300;1,400;1,500;1,600;1,700;1,800;1,900&display=swap");

@import url("https://fonts.googleapis.com/css2?family=DM+Sans:ital,wght@0,400;0,500;0,700;1,400;1,500;1,700&display=swap");
.container {
  width: 100%;
  height: 100%;
  background: #000;
  display: flex;
  justify-content: center;
}
.anualActive {
  display: flex;
  justify-content: center;
  align-items: center;
  width: 180px;
  color: #fff;
  height: 65px;
  background: #5454D4;
  border-radius: 10px 0px 0px 10px;
  font-family: "DM Sans", serif;
  font-style: normal;
  font-weight: bold;
  font-size: 16px;
  line-height: 21px;

  text-align: center;
  letter-spacing: -0.500211px;
  border: 5px solid #fff;
}
.mensalActive {
  display: flex;
  justify-content: center;
  align-items: center;
  width: 180px;
  color: #fff;
  height: 65px;
  background: #5454D4;
  border-radius: 0px 10px 10px 0px;
  font-family: "DM Sans", serif;
  font-style: normal;
  font-weight: bold;
  font-size: 16px;
  line-height: 21px;

  text-align: center;
  letter-spacing: -0.500211px;
  border: 5px solid #fff;
}
.anualDeactive {
  display: flex;
  justify-content: center;
  align-items: center;
  width: 180px;
  color: #AEAEAE;
  height: 65px;
  background: #fff;
  border-radius: 10px 0px 0px 10px;
  font-family: "DM Sans", serif;
  font-style: normal;
  font-weight: bold;
  font-size: 16px;
  line-height: 21px;

  text-align: center;
  letter-spacing: -0.500211px;
  border: 5px solid #fff;
  border-right: none;
}
.mensalDeactive {
  display: flex;
  justify-content: center;
  align-items: center;
  width: 180px;
  color: #AEAEAE;
  height: 65px;
  background: #fff;
  border-radius: 0px 10px 10px 0px;
  font-family: "DM Sans", serif;
  font-style: normal;
  font-weight: bold;
  font-size: 16px;
  line-height: 21px;

  text-align: center;
  letter-spacing: -0.500211px;
  border: 5px solid #fff;
  border-left: none;
}

.title {
  font-family: "DM Sans", serif;
  font-style: normal;
  font-weight: bold;
  font-size: 60px;
  /* or 117% */

  letter-spacing: -1.87579px;

  color: #AEAEAE;
}
.cardTitle {
  font-family: "DM Sans", serif;
  font-style: normal;
  font-weight: normal;
  font-size: 18px;
  /* identical to box height, or 156% */

  text-align: center;
  letter-spacing: -0.562737px;

  color: #000000;
}
.price {
  font-family: "DM Sans", serif;
  font-style: normal;
  font-weight: bold;
  font-size: 60px;
  line-height: 30px;
  /* identical to box height, or 93% */

  text-align: center;
  letter-spacing: -1.03448px;

  color: rgba(255, 255, 255, 0.8);
}
.paragraph {
  font-family: "Mulish", serif;
  font-style: normal;
  font-weight: normal;
  font-size: 17px;
  /* or 294% */

  text-align: center;
  letter-spacing: -0.531474px;

  color: #000000;
}
.plano {
  font-family: "DM Sans", serif;
  font-style: normal;
  font-weight: bold;
  font-size: 28px;
  line-height: 56px;
  /* identical to box height, or 200% */

  text-align: center;
  letter-spacing: -1.03448px;

  color: #FFFFFF;
}
.firstCard {
  padding: 1rem;
  width: 330px;
  height: 441px;
  background: linear-gradient(
    180deg,
    #FFFFFF 0%,
    rgba(255, 255, 255, 0) 96.64%
  );
}
.secondCard {
  padding: 1rem;
  width: 376px;
  height: 473px;
  background: linear-gradient(180deg, #CACAFF 0%, rgba(84, 84, 212, 0) 90.91%);
}
.thirdCard {
  padding: 1rem;
  width: 396px;
  height: 497px;
  background: linear-gradient(180deg, #6969FF 0%, rgba(84, 84, 212, 0) 90.91%);
}
.StartedButton {
  background: #5454D4;
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
