<template lang="">
    <div class="FAQ">
        <h2 class="faqHead">
            Frequently Ask Questions
        </h2>
        <img :src="greenLine" alt="" class="greenline" v-motion-slide-visible-top>
        <div class="accFlex">
            <div class="Wrap" id="app">
            <div class="">
                <AccordionVue title="Do you have a setup cost?" class="Wrap">
                <h2 class="costAcc">Mass-edit product prices smoothly in the dashboard set desired profit margin and let the app calculate and update prices in a swift minute to the webshop</h2>
                </AccordionVue>
                <AccordionVue title="Do you have a setup cost?" class="Wrap">
                <h2 class="costAcc">Mass-edit product prices smoothly in the dashboard set desired profit margin and let the app calculate and update prices in a swift minute to the webshop</h2>
                </AccordionVue>
                <AccordionVue title="Do you have a setup cost?" class="Wrap">
                <h2 class="costAcc">Mass-edit product prices smoothly in the dashboard set desired profit margin and let the app calculate and update prices in a swift minute to the webshop</h2>
                </AccordionVue>
                
            </div>
        </div>
        <div  id="app">
            <div class="">
                <AccordionVue title="Do you have a setup cost?" class="Wrap">
                <h2 class="costAcc">Mass-edit product prices smoothly in the dashboard set desired profit margin and let the app calculate and update prices in a swift minute to the webshop</h2>
                </AccordionVue>
                <AccordionVue title="Do you have a setup cost?" class="Wrap">
                <h2 class="costAcc">Mass-edit product prices smoothly in the dashboard set desired profit margin and let the app calculate and update prices in a swift minute to the webshop</h2>
                </AccordionVue>
                <AccordionVue title="Do you have a setup cost?" class="Wrap">
                <h2 class="costAcc">Mass-edit product prices smoothly in the dashboard set desired profit margin and let the app calculate and update prices in a swift minute to the webshop</h2>
                </AccordionVue>
                
            </div>
        </div>
        </div>
    </div>
    <div class="intelligent">
        <img :src="IntelligetImg" alt="" class="IntelligetImg">
        <h1 class="intelliText">
            Imexta is a Business Intelligence web application aiming to provide an intuitive,
            and easy reporting tool which allows for high level of dashboard and report
            customization. Imexta queries feeds from users accounting program and
            presents business metrics for cash flow forecasts, budgets, KPI’s etc. It also allows
            for user to simulate decisions and play with predictive scenarios.

        </h1>
        <ButtonVue class="Faqbtn" />
        <img :src="redLine" alt="" class="RedLine" v-motion-roll-visible-left>
    </div>
</template>
<script>
import AccordionVue from "./Accordion.vue";
import ButtonVue from "../Button.vue";
export default {
  name: "FaqVue",
  data() {
    return {
        IntelligetImg:require("../../../assets/intelligent.svg"),
        redLine:require("../../../assets/redLine.svg"),
        greenLine:require("../../../assets/greenline.svg"),

    }
  },
  components: {
    AccordionVue,
    ButtonVue
  },
};
</script>
<style scoped>
.FAQ {
  width: 100%;
  padding-top: 2%;
  margin-top: 20px;
}
.faqText {
  font-family: "Rubik";
  font-style: normal;
  font-weight: 500;
  font-size: 38px;
  line-height: 140%;
  text-align: center;

  color: #1a232d;
}
.Wrap {
  display: inline-flex;
  flex-direction: column;
  overflow: hidden;
  justify-content: center;
  align-content: center;
}

.costAcc {
  margin-left: 17%;
  font-family: "Rubik";
  font-style: normal;
  font-weight: 400;
  font-size: 15px;
  line-height: 40px;
  color: #1d467b;

  width: 100%;
}
.accFlex {
  display: inline-flex;
  width: 100%;
  overflow: hidden;
}
.intelligent{
    position: relative;
    width: 100%;
    /* height: 700px; */
    display: inline-flex;
    flex-direction: row;
    justify-content: center;
    top: 50px;
    align-items: center;
}
.IntelligetImg{
position: absolute;
width: 100%;
left: 0px;
top: 0px;
/* z-index: -122; */

}
.intelliText{
/* Imexta is a Business Intelligence web application aiming to provide an intuitive, and easy reporting tool which allows for high level of dashboard and report customization. Imexta queries feeds from users accounting program and presents business metrics for cash flow forecasts, budgets, KPI’s etc. It also allows for user to simulate decisions and play with predictive scenarios. */

position: absolute;
width: 80%;
height: 80px;
/* left: 26px; */
top: 30px;

font-family: 'Rubik';
font-style: normal;
font-weight: 400;
font-size: 25px;
line-height: 56px;
/* or 175% */
text-align: center;

/* Neutral/900 */
color: #1A232D;
}
.Faqbtn{
    /* Rectangle 150 */

position: absolute;

left: 540px;
top:330px;
border-radius: 8px;

    z-index: 2;
}
.RedLine{
    /* Vector */

position: absolute;
width: 300px;
left: 37%;
right: 34.53%;
top: 390px;
bottom: 120px;
  transition: .7s all ease-in-out;

}
.greenline{
    transition: .7s all ease-in-out;
    width: 23%;
}
</style>