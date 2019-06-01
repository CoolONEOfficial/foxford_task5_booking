<template>
    <!--TODO: cookie message-->
    
    <div class="fix" id="elm2">
      <div class="container-cookie">
        <div class="cookie-text"><span>В целях обеспечения наилучшего пользовательского опыта для вас мы собираем и используем </span><a href="https://www.booking.com/general.ru.html?aid=375440;label=yandex-fAeMqEnXAC%2AdldAeWbOMuQ-4506493104;sid=bba30412f9f5614ae3b5065bacb0a08b;tmpl=docs/privacy-policy;from_cb=1" style="color:white">cookie-файлы</a><span> и некоторые другие данные на нашем сайте в технических, аналитических и маркетинговых целях. Продолжая просмотр нашего сайта, вы соглашаетесь на сбор и использование cookie-файлов и других данных нами в соответствии с </span><a href="https://www.booking.com/general.ru.html?aid=375440;label=yandex-fAeMqEnXAC%2AdldAeWbOMuQ-4506493104;sid=bba30412f9f5614ae3b5065bacb0a08b;tmpl=docs/privacy-policy;from_cb=1" style="color:white">Положением о конфиденциальности</a>.</div>
        <button class="ck" id="btnclose">Закрыть</button>
      </div>
    </div>
    
</template>

<script>
    export default {
        name: "CookieMessage"
    }
    document.getElementById('btnclose').onclick = function(){
  document.getElementById('elm2').style.display = 'none';
}
</script>

<style scoped lang="scss">
    @import "../styles/colors";
  .fix{
  position: fixed;
  top: calc(100% - 110px);
  opacity: .75;
  height: 100%;
  background-color: #003580;
  margin: -8px;
  min-width: 700px;
}
.container-cookie{
  position: relative;
  background-color: #003580;
  text-align: center;
  min-width: 700px;
}
.cookie-text{
  position: relative;
  width: 90%;
  color: white;
  font-size: 13px;
  padding: 10px 0;
  text-align: center;
  left: 5%;
}
.ck{
  color: white;
  background-color: #07c;
  border-radius: 10px;
  position: relative;
  width: 100px;
  height: 30px;
  top: 5%;
  cursor: pointer;
  font-size: 13px;
  text-align: center;
  font-weight: bold;
}
.ck:hover{
  background-color: #01c; 
}


</style>

