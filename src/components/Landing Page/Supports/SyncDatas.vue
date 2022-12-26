<template lang="">
  <div class="syncdatas">
    <SyncData
      :Sync="Sync"
      syncText="Sync data from Google sheets"
      :Screenshot="Screenshot"
    />
  
      <SyncData
        :Sync="Sync1"
        syncText="Sync data to accounting your program"
        flexDir="row-reverse"
        marginLeft="105px"
        :Screenshot="Screenshot1"
        class="greenBag"
      />
      <SyncData
        :Sync="Sync2"
        syncText="Sync data from your accounting program"
        :Screenshot="Screenshot2"
        marginRight="105px"
        class="greenBag"
      />

    <SyncData
      :Sync="Sync3"
      syncText="Automatic invoice actions"
      flexDir="row-reverse"
      marginLeft="105px"
      :Screenshot="Screenshot3"
    />
  </div>
</template>
<script>
import SyncData from "@/components/Landing Page/Supports/SyncData.vue";
export default {
  name: "SyncDatas",
  data() {
    return {
      Sync: [],
      Sync1: [],
      Sync2: [],
      Sync3: [],
      Screenshot: require("../../../assets/googleData.svg"),
      Screenshot1: require("../../../assets/accounting.svg"),
      Screenshot2: require("../../../assets/timeline.svg"),
      Screenshot3: require("../../../assets/invoice.svg"),
    };
  },
  created() {
    (this.Sync = [
      {
        DragDrop: require("../../../assets/dragDrop.svg"),
        DragTxt:
          "Drag & Drop type of Dashboard with customizable graphs configuration",
      },
      {
        DragDrop: require("../../../assets/report.svg"),
        DragTxt:
          "PDF Report generation tool with the customized graphs+added text",
      },
      {
        DragDrop: require("../../../assets/mail.svg"),
        DragTxt: "Email inbox notification/alerts for key metrics activity",
      },
    ]),
      (this.Sync1 = [
        {
          DragDrop: require("../../../assets/cashFlow.svg"),
          DragTxt: "Cash flow forecasts",
        },
        {
          DragDrop: require("../../../assets/prediction.svg"),
          DragTxt: "Prediction and Prognosis",
        },
        {
          DragDrop: require("../../../assets/decision.svg"),
          DragTxt:
            "Decision simulation / Modelling of best case or worst case scenario",
        },
      ]),
      (this.Sync2 = [
        {
          DragDrop: require("../../../assets/dataRev.svg"),
          DragTxt: "Revenue granular overview",
        },
        {
          DragDrop: require("../../../assets/expense.svg"),
          DragTxt: "Expense granular overview and KPIs",
        },
        {
          DragDrop: require("../../../assets/highLevel.svg"),
          DragTxt: "High level user permission management ",
        },
      ]),
      (this.Sync3 = [
        {
          DragDrop: require("../../../assets/collaboration.svg"),
          DragTxt: "Collaboration/Sharing Dashboard with Accountant",
        },
        {
          DragDrop: require("../../../assets/customization.svg"),
          DragTxt: "User customization",
        },
        {
          DragDrop: require("../../../assets/multitenancy.svg"),
          DragTxt: "Multitenancy",
        },
      ]);
  },
  components: {
    SyncData,
  },
};
</script>
<style scoped>
.greenBag {
  background: #2da55f66;
}
</style>
