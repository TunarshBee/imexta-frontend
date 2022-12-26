<template lang="en">
    <nav class="navbar" >
      <img :src="Logo" alt="Imexta Logo" class="logo"/>
    <ul class="list-group" >
      <li class="list-group-items" > <a href="!#" class="navLink" >Features</a> </li>
      <li class="list-group-items" > <a href="!#" class="navLink" >About Us</a> </li>
      <li class="list-group-items" > <a href="!#" class="navLink" >Contact</a> </li>
      <li class="list-group-items" > <a href="!#" class="navLink" >Princing</a> </li>
      <li class="list-group-items" > <a href="!#" class="navLink" >Blog</a> </li>
    </ul>
    <button class="btn" > Login/Signup</button>
    </nav>
</template>

<script>
export default {
  name: "NavBar",
  data() {
    return {
      Logo: require("../../assets/logo.svg"),
    };
  },
};
</script>
<style scoped>

.navbar {
  position: absolute;
  width: 100%;
  height: 70px;
  left: 0px;
  top: 0px;
  display: inline-flex;
  justify-content: center;
  justify-items: baseline;
  background: #ffffff;
  box-shadow: 0px 7px 40px rgba(0, 0, 0, 0.12);
}
.logo {
  position: absolute;
  width: 169px;
  height: 48px;
  left: 39px;
  top: 11px;
  border-radius: 5px;
}
.list-group {
  display: inline-flex;
  width: 70%;
  padding-left: 30%;
  align-items: center;
  justify-content: space-evenly;
}
.navLink {
  /* Features */
  font-family: "Rubik";
  font-style: normal;
  font-weight: 400;
  font-size: 20px;
  line-height: 20px;
  text-decoration: none;
  color: #1a232d;
}
.btn {
  display: inline;
  align-self: center;
  width: 138px;
  height: 48px;
  background: #eaf1fa;
  border: none;
  border-radius: 4px;
  margin-left: 2%;
  /* Login/Signup */



font-family: 'Rubik';
font-style: normal;
font-weight: 500;
font-size: 18px;
line-height: 21px;

/* Primary/300 */
color: #4583D3;


}
</style>