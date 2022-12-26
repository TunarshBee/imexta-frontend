<template lang="">
    <div class="pricing">
        <div>
            <h1 class="pricingText">
            Our pricing
            </h1>
            <img :src="GreenLine" alt="" class="greenLine" v-motion-roll-visible-left>
            <h3 class="paymentPeriod">Choose payment period and amount of transactions monthly to see your final monthly price</h3>
        <select name="" id="perid">
            <option value="Period">Payment Period</option>
        </select>
        <select name="" id="perid">
            <option value="Amount">Amount of transactions</option>
        </select>
        </div>  
        <div class="pricingCards">
            <div class="card1">
                <h1 class="cardText">Basic</h1>
                <h1 class="cardPrice">$30 <small>/month</small></h1>
                <h3 class="vat">price excl. VAT</h3>
                <ButtonVue v-motion-fade-visible class="bttn" />
                <ul class="features">Features :
                  <li class="featuresList">
                    <img :src="GreenTick" alt="" class="greentick">
                    Feature 1</li>
                  <li class="featuresList">
                    <img :src="GreenTick" alt="" class="greentick">
                    Feature 2</li>
                  <li class="featuresList">
                    <img :src="GreenTick" alt="" class="greentick">
                    Feature 3</li>
                  <li class="featuresList">
                    <img :src="GreenTick" alt="" class="greentick">
                    Feature 4</li>
                  <li class="featuresList">
                    <img :src="GreenTick" alt="" class="greentick">
                    Feature 5</li>
                </ul>
            </div>
            <div class="card2">
                <h1 class="cardText">Basic</h1>
                <h1 class="cardPrice">$30 <small>/month</small></h1>
                <h3 class="vat">price excl. VAT</h3>
                <ButtonVue v-motion-fade-visible class="bttn" />
                <ul class="features">Features :
                  <li class="featuresList">
                    <img :src="WhiteTick" alt="" class="greentick">
                    Feature 1</li>
                  <li class="featuresList">
                    <img :src="WhiteTick" alt="" class="greentick">
                    Feature 2</li>
                  <li class="featuresList">
                    <img :src="WhiteTick" alt="" class="greentick">
                    Feature 3</li>
                  <li class="featuresList">
                    <img :src="WhiteTick" alt="" class="greentick">
                    Feature 4</li>
                  <li class="featuresList">
                    <img :src="WhiteTick" alt="" class="greentick">
                    Feature 5</li>
                  <li class="featuresList">
                    <img :src="WhiteTick" alt="" class="greentick">
                    Feature 6</li>
                </ul>
            </div>
            <div class="card1">
                <h1 class="cardText">Basic</h1>
                <h1 class="cardPrice">$30 <small>/month</small></h1>
                <h3 class="vat">price excl. VAT</h3>
                <ButtonVue v-motion-fade-visible class="bttn" />
                <ul class="features">Features :
                  <li class="featuresList">
                    <img :src="GreenTick" alt="" class="greentick">
                    Feature 1</li>
                  <li class="featuresList">
                    <img :src="GreenTick" alt="" class="greentick">
                    Feature 2</li>
                  <li class="featuresList">
                    <img :src="GreenTick" alt="" class="greentick">
                    Feature 3</li>
                  <li class="featuresList">
                    <img :src="GreenTick" alt="" class="greentick">
                    Feature 4</li>
                  <li class="featuresList">
                    <img :src="GreenTick" alt="" class="greentick">
                    Feature 5</li>
                </ul>
            </div>
        </div>
    </div>
</template>
<script>
import ButtonVue from "../Button.vue";
export default {
  name: "PricingPage",
  components: {
    ButtonVue,
  },
  data() {
    return {
      GreenLine: require("../../../assets/greenline.svg"),
      GreenTick: require("../../../assets/greenTick.svg"),
      WhiteTick: require("../../../assets/whiteTick.svg"),
    };
  },
};
</script>
<style scoped>
.pricing {
  width: 100%;
  
}
.pricingCards{
  margin-top: 10%;
  display:flex;
  justify-content: space-evenly;
}
.pricingText {
  font-family: "Rubik";
  font-style: normal;
  font-weight: 500;
  font-size: 38px;
  line-height: 140%;
  text-align: center;
  color: #1a232d;
  margin-bottom: -1%;
}
.greenLine {
  width: 15%;
    transition: .5s all ease-in-out;

}
.paymentPeriod {
  font-family: "Rubik";
  font-style: normal;
  font-weight: 400;
  font-size: 20px;
  line-height: 140%;
  color: #2c3a4b;
}
#perid {
  /* Rectangle 6070 */

  box-sizing: border-box;
  width: 275px;
  height: 45px;
  padding: 1% 0.3%;
  background: #ffffff;
  border: 0.8px solid #2da55f;
  box-shadow: 0px 2px 8px rgba(184, 184, 184, 0.25);
  border-radius: 5px;
  font-family: "Roboto";
  font-style: normal;
  font-weight: 400;
  font-size: 17px;
  line-height: 26px;
  color: rgba(35, 45, 57, 0.5);
}
#perid:last-child {
  margin-left: 5%;
}
.card1 {
  margin: auto;
  width: 25%;
  height: fit-content;
  /* padding: 2%; */
  border-radius: 24px;
  display: inline-flex;
  flex-direction: column;
  background: #ffffff;
  box-shadow: 0px 7px 40px rgba(0, 0, 0, 0.12);
  color: #2da55f;
}
.card2 {
  /* margin: auto; */
  margin-top: -3.5%;
  width: 25%;
  height: fit-content;
  /* padding: 2%; */
  border-radius: 24px;
  display: inline-flex;
  flex-direction: column;
  background: #2da55f;
  box-shadow: 0px 7px 40px rgba(0, 0, 0, 0.12);
  color: #fff;
}
.cardText {
  font-family: "Rubik";
  font-style: normal;
  font-weight: 500;
  font-size: 17px;
  line-height: 28px;
  margin-top: 30px;
}
.cardPrice {
  font-family: "Rubik";
  font-style: normal;
  font-weight: 700;
  font-size: 32px;
}
.cardPrice > small {
  font-family: "Rubik";
  font-style: normal;
  font-weight: 700;
  font-size: 18px;
}
.vat {
  font-family: "Rubik";
  font-style: normal;
  font-weight: 400;
  font-size: 20px;

  margin-bottom: 20px;
}
.bttn {
  margin: auto;
}
.bttn:hover{
  border: 1px solid green;
  color:#FBD531;
  background-color: #fff;
}
.features {
  font-family: "Rubik";
  font-style: normal;
  font-weight: 500;
  font-size: 20px;
  line-height: 28px;
  margin: 20px 50px;

  /* margin-left: -20%; */
  text-align: start;
  display: inline-flex;
  flex-direction: column;
  justify-content: right;
}
.featuresList {
  font-family: "Rubik";
  font-style: normal;
  font-weight: 400;
  font-size: 20px;
  line-height: 28px;
  margin-top: 20px;
}
.greentick {
  width: 15px;
}
</style>