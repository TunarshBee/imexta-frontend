<template lang="">
    <div class="section1" >
        <div class="aside">
            <h1 class="header">90%</h1>
            <h3 class="bus">of small businesses fail within the first 5 years </h3>
            <h2 class="reason">What is the reason?</h2>
            <img :src="RedLine" alt="" srcset="" class="redline" v-motion-roll-visible-left>
        </div>
        <img :src="RedArrow" alt="" srcset="" class="redArrow" v-motion-slide-visible-left>
        <div class="rightAside">
            <h3 class="causes">
                One of the main causes being the
                missing of eagle eye<br/> watch of the business cash flow and taking financial <br/>decisions
                before-hand of a potential crisis/loss. Preventive, <br/>informed action combined with a steady
                oversight of the<br/> key metrics of the company is a necessity to stay alive in <br/> the present tough market.
            </h3>

            <h2 class="solution">
                The solution?
            </h2>
            <img :src="GreenLine" alt="" srcset="" class="greenline" v-motion-roll-visible-right>
        </div>
        <img :src="GreenArrow" alt="" srcset="" class="greenarrow" v-motion-slide-visible-right>

    </div>
</template>

<script>
export default {
	name: "SectionThree",
	data() {
		return {
			RedLine: require("../../../assets/redLine.svg"),
			RedArrow: require("../../../assets/redArrow.svg"),
			GreenArrow: require("../../../assets/greenArrow.svg"),
			GreenLine: require("../../../assets/greenline.svg"),
		};
	},
};
</script>

<style scoped>
.section1 {
	widows: 100%;
	padding-left: 12%;
}
.section1 > .aside {
	width: 27%;
	text-align: start;
}
.section1 > .aside > .header {
	font-family: "Rubik";
	font-style: normal;
	font-weight: 700;
	font-size: 50px;
	line-height: 120px;
	color: #1a232d;
}
.bus {
	width: 280px;
	height: 50px;

	font-family: "Rubik";
	font-style: normal;
	font-weight: 400;
	font-size: 18px;
	line-height: 130%;
	/* or 62px */

	/* Neutral/900 */
	color: #1a232d;
}
.reason {
	width: 602px;
	height: 37px;

	font-family: "Rubik";
	font-style: normal;
	font-weight: 500;
	font-size: 35px;
	line-height: 130%;
	/* or 83px */

	/* Neutral/900 */
	color: #1a232d;
}
.redline {
	left: 8.33%;
	right: 60.31%;
	top: 14.61%;
	bottom: 85.28%;
	width: 100%;
  transition: .4s all ease-in-out;
}
.redArrow {
	width: 10%;
	transition: linear 0.8s all cubic-bezier(0.19, 1, 0.22, 1);
	position: absolute;
	left: 45%;
	top: 860px;
	bottom: 13.02%;
}
.rightAside {
	width: 80%;
	display: inline-flex;
	flex-direction: column;
	justify-content: end;
	align-items: flex-end;
}
.causes {
	width: 80%;
	margin-top: 70px;
	font-family: "Rubik";
	font-style: normal;
	font-weight: 500;
	font-size: 17px;
	line-height: 140%;
	text-align: right;
	color: #1a232d;
}
.solution {
	font-family: "Rubik";
	font-style: normal;
	font-weight: 500;
	font-size: 34px;
	line-height: 130%;

	text-align: right;

	color: #1a232d;
}
.greenline {
	width: 23%;
    transition: .4s all ease-in-out;

}
.greenarrow {
	width: 200px;
	position: absolute;
	left: 46.41%;
  transition: .7s all ease-in-out;
	right: 20.35%;
	top: 1120px;
	bottom: -42.81%;
	z-index: 1;
}
</style>