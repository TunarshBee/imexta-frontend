<template lang="">
    <footer class="footer">
       <div class="top">
            <div class="first">
                <img :src="Logo" alt="" class="Logo">
                <h1 class="footerText">
                    Imexta is a Business Intelligence web application aiming to provide an intuitive,
                    and easy reporting tool which allows for high level of dashboard and report
                    customization. Imexta queries feeds from users accounting program and
                    presents business metrics for cash flow forecasts, budgets, KPI’s etc. It also allows
                    for user to simulate decisions and play with predictive scenarios.
                </h1>
            </div>
            <div class="second">
                <ul class="secondList">
                    <h1>Resources</h1>
                    <li class="secondListItem"><a href="#">Login</a></li>
                    <li class="secondListItem"><a href="#">FAQ</a></li>
                    <li class="secondListItem"><a href="#">Blog</a></li>
                    <li class="secondListItem"><a href="#">Prices</a></li>
                    <li class="secondListItem"><a href="#">Get started</a></li>
                    <li class="secondListItem"><a href="#">Terms & Condition</a></li>
                    
                </ul>
            </div>
            <div class="third">
                <ul class="thirdList">
                    <h1>Resources</h1>
                    <li class="thirdListItem"><a href="#">Import data to accounting program</a></li>
                    <li class="thirdListItem"><a href="#">Export data from accounting program</a></li>
                    <li class="thirdListItem"><a href="#">Sync data from Google Sheets to accounting program</a></li>
                    <li class="thirdListItem"><a href="#">Auto-bookkeep generated invoices</a></li>
                    <li class="thirdListItem"><a href="#"> Auto-send generated invoices</a></li>
                    
                    
                </ul>
            </div>
       </div>
       <div class="copyright">© 2022 Imexta. All rights reserved</div>
    </footer>
</template>
<script>
export default {
    name:"FooterVue",
    data() {
        return {
      Logo: require("../../assets/logo.svg"),
            
        }
    },
}
</script>
<style scoped>
a{
    text-decoration: none;
    color: #DBDBDB;
    
}
.footer {
    position: relative;
    top: 480px;
    width: 100%;
    background: #008337;
    display: inline-flex;
    flex-direction: column;
    justify-content: space-evenly;
    align-items: baseline;
    padding: 4% 0;
    bottom: 50  px;
}
.footer .top{
    top: 480px;
    width: 100%;
    display: inline-flex;
    justify-content: space-evenly;
    align-items: baseline;

}
.top > .first{
    display: inline-flex;
    flex-direction: column;
    width:30%;
    justify-content: center ;
    align-items: flex-start;
    text-align: start;
    
}
.top > .second, .top > .third{
    display: inline-flex;
    flex-direction: column;
    width:fit-content;
    justify-content: center ;
    align-items: flex-start;
    text-align: start;
    
}


.secondList, .thirdList{
font-family: 'Rubik';
font-style: normal;
font-weight: 400;
font-size: 18px;
/* line-height: 18px; */
color: #DBDBDB;
}
.secondListItem, .thirdListItem{
font-family: 'Rubik';
font-style: normal;
font-weight: 400;
font-size: 12px;
/* line-height: 18px; */
margin-top: 15%;
color: #DBDBDB;


}
.thirdListItem{
    
    margin-top: 10%;
}
.footerText{
font-family: 'Rubik';
font-style: normal;
font-weight: 400;
font-size: 12px;
line-height: 28px;

color: #DBDBDB;


}
.copyright{
    padding-left: 8.5%;
    color: #DBDBDB;
}
</style>