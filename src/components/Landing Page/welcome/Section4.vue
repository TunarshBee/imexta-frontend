<template lang="">
	<div class="section4" >
		<span>
			<img :src="GreenBack" alt="" srcset="" class="greenback">
		<h2 class="service">
			Imexta aims to service the Nordic SME’s with an affordable option, bringing data analysis and BI to the common man.

		</h2>
		</span>
		<img :src="revenue" alt="revenue Screeshot" srcset="" class="revenue" v-motion-slide-visible-bottom >
	</div>
</template>
<script>
export default {
  name: "SectionFour",
  data() {
    return {
      GreenBack: require("../../../assets/greenBack.svg"),
      revenue: require("../../../assets/revenue.svg"),
    };
  },
};
</script>
<style scoped>
.section4 {
  width: 80%;
  margin-left: 3%;
  position: relative;
  margin-top: 5%;
  display: inline-flex;
  flex-direction: column;
  align-items: center;
  justify-content: center;
  text-align: center;
}
.greenback {
  width: 100%;
  border-radius: 20px;
}
.service {
  position: absolute;
  width: 547px;
  height: 156px;
  left: 25%;
  top: 50px;

  font-family: "Rubik";
  font-style: normal;
  font-weight: 700;
  font-size: 25px;
  line-height: 130%;
  text-align: center;

  color: #f7f8fa;
}
.revenue {
  position: absolute;
  top: 45%;
  width: 70%;
  box-shadow: 0px 0px 80px rgba(0, 0, 0, 0.12);
}
</style>