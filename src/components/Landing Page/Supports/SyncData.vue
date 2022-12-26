<template lang="">
  <div
    class="syncData"
    :style="{ 'flex-direction': flexDir, 'padding-left': marginLeft, 'padding-right': marginRight}"
  >
    <img
      :src="Screenshot"
      alt=""
      srcset=""
      class="googleData"
      :style="{ 'margin-right': marginRig }"
      v-motion-pop-visible
    />

    <div class="dataList" >
      <h1 class="syncText">
        {{ syncText }}
      </h1>
      <ul class="syncList" v-for="(Syn, index) in Sync" :key="index" >
        <li class="syncListItems" v-motion-slide-visible-bottom>
          <img :src="Syn.DragDrop" alt="" srcset="" />
          <h3 class="syncListItemsText">{{ Syn.DragTxt }}</h3>
        </li>
      </ul>
      <a href="!#" class="anchor">
        Learn More
        <i class="fa-solid fa-arrow-right"></i>
      </a>
    </div>
  </div>
</template>
<script>
export default {
  name: "SyncDataVue",
  data() {
    return {
      DragDrop: require("../../../assets/dragDrop.svg"),
    };
  },
  props: {
    Sync: Array,
    syncText: String,
    flexDir: String,
    Screenshot: String,
    marginLeft: String,
    marginRight: String,
  },
};
</script>
<style scoped>
.syncData {
  width: 100%;
  display: inline-flex;
  justify-content: space-between;
  align-items: center;
  text-align: start;
}
.googleData {
  width: 55%;
  margin-left: .2%;
  transition: linear .4s cubic-bezier(0.075, 0.82, 0.165, 1);
}
.syncText {
  font-family: "Rubik";
  font-style: normal;
  font-weight: 700;
  font-size: 20px;
  line-height: 130%;
  color: #1a232d;
  text-align: start;
}

.syncListItems {
  display: inline-flex;
  flex-direction: row;
  justify-content: flex-start;
  align-items: center;
  text-align: start;
  width: 100%;
  /* background-color: aliceblue;  */
}
.syncListItems > img {
  height: 100px;
}
.syncListItemsText {
  width: 50%;
  text-align: start;
  font-family: "Rubik";
  font-style: normal;
  font-weight: 400;
  font-size: 15px;
  line-height: 140%;
  color: #1a232d;
}
.syncList > a {
  margin-top: 3%;
}
.syncList > a:last-child {
  margin-bottom: 3%;
}
.anchor {
  font-family: "Rubik";
  font-style: normal;
  font-weight: 500;
  font-size: 17px;
  line-height: 24px;

  text-decoration-line: underline;
  color: #1d467b;
}
.dataList {
  display: inline-flex;
  flex-direction: column;
}
</style>
