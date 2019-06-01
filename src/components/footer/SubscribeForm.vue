<template>
    <!--TODO: subscribe form-->  
    
    <div class="container1111">
    <div class="container111">
    <div class="text111">Сэкономьте время и деньги!</div>
    <div class="text222">Подпишитесь, и мы вышлем вам лучшие предложения </div>
    <input type="input" class="inpt" placeholder="Ваш электронный адрес"></input>
    <button class="sbscr">Подписаться</button>
    </div>
  <div class="cbx"><input type="checkbox" class="chb" unchecked></input>
  <label class="chbx">Отправить мне ссылку для загрузки БЕСПЛАТНОГО приложения Booking.com</label></div>
  </div>
  
</template>

<script>
    export default {
        name: "SubscribeForm"
    }

</script>

<style scoped lang="scss">
    @import "../../styles/colors";
.container1111{
  font-family: Segoe UI;
  width: 100%;
  height: 300px;
  background-color: #001b42;
  margin: -8px;
  text-align: center;
  min-width: 600px;
}
.container111{
  width: 100%;
  height: 160px;
  margin: -8px;
  background-color: #001b42;
  text-align: center;
}
.sbscr{
  cursor: pointer;
  color: white;
  background-color: #07c;
  margin-left: auto;
  margin-right: auto;
  position: relative;
  border-radius: 3px;
  border: 0;
  padding: 0 15px;
  font-size: 20px;
  height: 48px;
  width: 200px;
}
.sbscr:hover{
  background-color: #05c;
}
.inpt{
  position: relative;
  margin-left: auto;
  margin-right: auto;
  font-size: 20px;
  line-height: 28px;
  color: #707070;
  border: 0;
  border-radius: 3px;
  padding: 10px;
  width: 350px;
}
.chbx{
  position: relative;
  color: white;
  font-size: 13px;
  margin-left: 15px;
  padding-left: 8px;
  top: -2px;
}
.cbx{
  position: relative;
  left: -50px;
  top: 6px; 
}
.chb{
  margin-left: -490px;
  position: absolute;
  width: 1000px;
  z-index: 100;
}
.text111{
  color: white;
  font-size: 24px;
  padding-top: 30px;
  font-weight: bold;
}
.text222{
  color: #bdbdbd;
  font-size: 16px;
  padding-bottom: 20px;
}

</style>


