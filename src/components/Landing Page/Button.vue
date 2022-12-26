<template lang="">
    <button class="getStarted" >
            Get Started
            <i class="fa-solid fa-arrow-right"></i>
        </button>
</template>
<script>

export default {
    name:"ButtonVue",
    
}
</script>
<style Scoped>
  .getStarted {
  width: 211px;
  height: 50px;
  left: 772px;
  top: 546px;
  border-radius: 8px;
  font-family: "Rubik";
  font-style: normal;
  font-weight: 500;
  font-size: 18px;
  line-height: 24px;
  cursor: pointer;
  border: none;
  color: #f7f8fa;
  box-shadow:  3px  10px 10px rgba(0, 0, 0, 0.12);
  background-color:#FBD531;

}
.getStarted:hover{
  border: 1px solid green;
  color:#FBD531;
  background-color: #fff;
}
</style>