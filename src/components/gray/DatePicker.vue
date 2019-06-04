<template>
<div>
<label id="Отъезд">Отъезд <input type="date" id="bday" name="bday" required pattern="[0-9]{4}-[0-9]{2}-[0-9]{2}">
    <span class="validity"></span></label>
<label  id="Заезд">Заезд   <input type="date" id="bday" name="bday" required pattern="[0-9]{4}-[0-9]{2}-[0-9]{2}">
    <span class="validity"></span></label>
    <div id="text">
    <h2>Найдите лучшие предложения</h2>
    <p id="text1">От уютных загородных домов до стильных городских квартир </p>
    </div>
    </div>
</template>

<script>
    export default {
        name: "DatePicker"
    }
</script>

<style scoped lang="scss">


#text1{
position: relative;
top: -15px;
}
#text {
position: absolute;
left: 130px;
}
label{
position: absolute;
top: 240px;
left: 625px;
 font-weight: bold;
 color: rgb(68,68,68);
 border: 1px solid rgba(0,0,0,.1);
 border-radius: 3px;
 background: rgb(245,245,245) linear-gradient(#f4f4f4, #f1f1f1);
   transition: all .218s ease 0s;
  z-index: 1;
}
label:hover {
color: rgb(24,24,24);
  border: 1px solid rgb(198,198,198);
  background: #f7f7f7 linear-gradient(#f7f7f7, #f1f1f1);
  box-shadow: 0 1px 2px rgba(0,0,0,.1);
}
label:active {
color: rgb(51,51,51);
border: 1px solid rgb(204,204,204);
background: rgb(238,238,238) linear-gradient(rgb(238,238,238), rgb(224,224,224));
box-shadow: 0 1px 2px rgba(0,0,0,.1) inset;
}
#Заезд{
left:470px;
height:25px;
width:185px;
font-size: 17px;
}
#Отъезд{
top:267px;
left:470px;
height:25px;
width:185px;
font-size: 16px;
}
input{
width: 110px;
font-size: 14px;
border: 1px solid #00000F;
background: #F6F6f6;
border-radius: 5px;
left:100px;
}

</style>
