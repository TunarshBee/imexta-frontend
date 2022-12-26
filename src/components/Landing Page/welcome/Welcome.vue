<template lang="">
    <section class="welcome">
        <h1 class="welcomeText">
            We aim to provide an intuitive and easy reporting tool
        </h1>
        <img :src="Line" alt="underline" class="line" >
        <h3 class="text2" >
            Which allows for high level of dashboard and report customization.
        </h3>
        <ButtonVue v-motion :initial="{opacity: 1, y: 0}"/>
    </section>
    <SectionTwo />
    <SectionThree/>
    <SectionFour/>
</template>
<script>
import SectionTwo from "@/components/Landing Page/welcome/Section2.vue"
import SectionThree from "@/components/Landing Page/welcome/Section3.vue"
import SectionFour from "@/components/Landing Page/welcome/Section4.vue"
import ButtonVue from "../Button.vue";

export default {
  name: "WelCome",
  data() {
    return {
      Line: require("../../../assets/greenline.svg"),
    };
  },
  components:{
    SectionTwo,
    SectionThree,
    SectionFour,
    ButtonVue,
  }
};
</script>
<style scoped>
.welcome {
  display: inline-flex;
  justify-content: center;
  flex-direction: column;
  align-items: center;
}

.welcomeText {
  margin-top: 7%;
  width: 60%;
  height: 140px;

  font-family: "Rubik";
  font-style: normal;
  font-weight: 700;
  font-size: 40px;
  line-height: 130%;
  text-align: center;
  color: #1a232d;
}
.line {
  width: 273px;

  position: absolute;
  left: 46.6%;
  right: 30.68%;
  top: 230px;
}
.text2 {
  width: 450px;
  height: 84px;

  font-family: "Rubik";
  font-style: normal;
  font-weight: 400;
  font-size: 22px;
  line-height: 130%;
  text-align: center;
  color: #2c3a4b;
}

</style>