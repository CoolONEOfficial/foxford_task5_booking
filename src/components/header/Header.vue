<template>
    <div class="abc">
        <!--TODO: header-->
        <v-layout row>
            <Search></Search>
            <CurrencySelection>
                 <div class="right-part">
                        <a id="currency" title="Выберите валюту">РУБ</a>
                 </div>
            </CurrencySelection>
            <LanguageSelection>
                <div class="right-part">
                    <a id="language" title="Выберите язык" role="button"><img src="https://r-ec.bstatic.com/static/img/flags/24/ru/88fbb4ed75a0daae6222ed2426e26cef1537eecd.png"></a>
                </div>
            </LanguageSelection>
        </v-layout>
        <div class="gh">
                    <div class="top-line">
                        <div class="left-part">
                            <img id="logotip" class src="https://q-ec.bstatic.com/static/img/b26logo/booking_logo_retina/22615963add19ac6b6d715a97c8d477e8b95b7ea.png" width="150px" height="25px">
                        </div>
                        <div class="right-part">
                            <div id="frame">Зарегестрировать свой объект</div>
                            <div id="reg-person">Зарегестрироваться</div>
                            <div id="log-in">Войти в аккаунт</div>
                        </div>

                    </div>
                    <div class="bottom-line">
                        <div id="btn1">Проживание</div>
                        <div id="btn2">Авиабилеты</div>
                        <div id="btn3">Аренда машин</div>
                        <div id="btn4">Такси от/до аэропорта</div>
                    </div>
            </div>
    </div>
</template>

<script>
    import CurrencySelection from "./CurrencySelection";
    import LanguageSelection from "./LanguageSelection";
    import Search from "../gray/Search";

    export default {
        name: "Header",
        components: {
            Search,
            LanguageSelection,
            CurrencySelection,
        },
    }
</script>

<style scoped lang="scss">
    @import "../../styles/colors";
    *{
        margin: 0px;
        padding: 0px;
        border: 0px;
        outline: 0;
    }

    template {
        background: #ffffff;
        margin: 0 auto;
    }

    .top-line {
        height: 50px;
        background-color: #003580;

    }

    #logotip {
        position: absolute;
        left: 5%;
        top: 12px;
    }

    .right-part {
        height: 50px;
        width: 70%;
        margin-left: 30%;
        position: relative;
        cursor: pointer;
    }

    #currency {
        float: left;
        font-size: 16px;
        font-weight: bold;
        position: absolute;
        color: #f1f1f1;
        display: block;
        text-decoration: none;
        top: 35%;
        font-family: BlinkMacSystemFont, Arial;			
    }

    #language {
        float: left;
        position: absolute;
        display: block;
        top: 29%;
        left: 9%;
    }

    .left-part {
        position: relative;
    }

    #frame:hover {
        background-color: #4682B4;
    }

    #frame {
        border: white solid 1px;
        border-radius: 3px;
        top: 20%;
        height: 18px;
        width: 22%;
        left: 20%;
        font-size: 12px;
        font-weight: bold;
        position: absolute;
        text-align: center;
        color: white;
        display: block;
        text-decoration: none;
        font-family: BlinkMacSystemFont, Arial;
        padding: 7px 10px;
    }

    #reg-person:hover,
    #log-in:hover {
        color: #4682B4;
    }

    #reg-person {
        border: white solid 1px;
        border-radius: 3px;
        background-color: white;
        top: 20%;
        height: 18px;
        width: 15%;
        left: 51%;
        font-size: 12px;
        font-weight: bold;
        position: absolute;
        color: #003580;
        display: block;
        text-decoration: none;
        font-family: BlinkMacSystemFont, Arial;
        padding: 7px 10px;
        text-align: center;
    }

    #log-in {
        border: white solid 1px;
        border-radius: 3px;
        background-color: white;
        top: 20%;
        height: 18px;
        width: 12%;
        left: 75%;
        font-size: 12px;
        font-weight: bold;
        position: absolute;
        color: #003580;
        display: block;
        text-decoration: none;
        font-family: BlinkMacSystemFont, Arial;
        padding: 7px 10px;
        text-align: center;
    }

    .bottom-line {
        background-color: #003580;
        height: 60px;
        width: 100%;
        top: 50px;
        position: absolute;
    }

    #btn1:hover,
    #btn2:hover,
    #btn3:hover,
    #btn4:hover {
        background-color: #4682B4;
    }

    #btn1 {
        height: 28px;
        width: 100px;
        background-color: #003580;
        border-radius: 3px;
        font-size: 15px;
        padding-top: 7px;
        padding-bottom: -2px;
        text-align: center;
        position: absolute;
        left: 5%;
        display: block;
        text-decoration: none;
        font-family: BlinkMacSystemFont, Arial;
        color: white;
        top: 12px;
        cursor: pointer;	
    }

    #btn2 {
        height: 28px;
        font-size: 15px;
        padding-top: 7px;
        width: 100px;
        background-color: #003580;
        border-radius: 3px;
        text-align: center;
        position: absolute;
        left: 15%;
        display: block;
        text-decoration: none;
        font-family: BlinkMacSystemFont, Arial;
        color: white;
        top: 12px;
        cursor: pointer;
    }

    #btn3 {
        height: 28px;
        font-size: 15px;
        padding-top: 7px;
        width: 120px;
        background-color: #003580;
        border-radius: 3px;
        text-align: center;
        position: absolute;
        left: 26%;
        display: block;
        text-decoration: none;
        font-family: BlinkMacSystemFont, Arial;
        color: white;
        top: 12px;
        cursor: pointer;
    }

    #btn4 {
        height: 28px;
        font-size: 15px;
        padding-top: 7px;
        width: 170px;
        background-color: #003580;
        border-radius: 3px;
        text-align: center;
        position: absolute;
        left: 39%;
        display: block;
        text-decoration: none;
        font-family: BlinkMacSystemFont, Arial;
        color: white;
        top: 12px;
        cursor: pointer;
    }
</style> 
