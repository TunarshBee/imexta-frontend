<template lang="">
    <section class="sec2">
        <h2 class="secText">
            It also allows
            for user to simulate decisions and
            play with predictive scenarios.

        </h2>
        <img :src="Section2" alt="Dashboard Screeshot" srcset="" class="dashboard"  >
    </section>
</template>
<script>
export default {
	name: "SectionT",
	data() {
		return {
			Section2: require("../../../assets/section2.svg"),
		};
	},
};
</script>
<style scoped>
.sec2 {
	position: relative;
	display: inline-flex;
	width: 100%;
	flex-direction: row;
	align-items: center;
	margin-top: 200px;
	padding-left: 12%;
	justify-items: baseline;
}
.secText {
	width: 330px;
	height: 80px;

	font-family: "Rubik";
	font-style: normal;
	font-weight: 400;
	font-size: 14px;
	line-height: 40px;
	color: #2c3a4b;
	text-align: start;
}
.dashboard {
	position: absolute;
	height: 700px;
	right: 20px;
}
</style>