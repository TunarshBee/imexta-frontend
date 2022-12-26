<template>
  <div id="app">
    <NavBar />
  <WelCome/>
  <SupportPlat/>
  <SyncDatas/>
  <PrincingVue/>
  <FAQVue/>
  <FooterVue/>
  </div>
</template>

<script>
import NavBar from "@/components/Landing Page/Nav.vue";
import WelCome from "@/components/Landing Page/welcome/Welcome.vue";
import SupportPlat from '@/components/Landing Page/Supports/Support.vue'
import PrincingVue from "./components/Landing Page/Pricing/Princing.vue";
import FAQVue from "./components/Landing Page/FAQ/FAQ.vue";
import FooterVue from "./components/Landing Page/Footer.vue";
import SyncDatas from '@/components/Landing Page/Supports/SyncDatas.vue'

export default {
  name: 'App',
  components:{
    NavBar,
    WelCome,
    SupportPlat,
    SyncDatas,
    PrincingVue,
    FAQVue,
    FooterVue,
  }
}
</script>

<style>
@import url('https://fonts.googleapis.com/css2?family=Rubik:ital,wght@0,300;0,400;0,500;0,600;0,700;0,800;0,900;1,300;1,400;1,500;1,600;1,700;1,800;1,900&display=swap');
* {
  box-sizing: border-box;
  margin: 0%;
  padding: 0%;
  outline: none;
  list-style: none;
  text-decoration: none;
}
#app {
  font-family: "Rubik",Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  background: #f5f5f5;
  margin-top: 60px;
}

</style>
