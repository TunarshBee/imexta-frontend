<template lang="">
    <div class="support" >
        <h1 class="platforms">Our supported integration platforms</h1>
        <div class="supportedPlatforms">
                <img :src="fortnox" alt="" class="supported" >
        </div>
    </div>
</template>
<script>
export default {
  name: "SuppotedPlat",
  data() {
    return {
      fortnox: require("../../../assets/fortnox.svg"),
    };
  },
};
</script>
<style scoped>
.support {
  position: relative;
  width: 100%;
  text-align: center;
  margin-top: 250px;
}
.platforms {
  font-family: "Rubik";
  font-style: normal;
  font-weight: 500;
  font-size: 40px;
  line-height: 140%;

  text-align: center;

  color: #1a232d;
}
.supportedPlatforms {
  width: 100%;
}
.supported {
  width: 100%;
  height: 303px;
  left: 96px;
}
</style>