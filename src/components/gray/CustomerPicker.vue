<template>
<div>
    <input type="checkbox" id="check">

    <label for="check" id="Cus"><p align="center"> взрослые  ·  дети  ·  номера</p> </label>
    <div class="popup">
    <div id="textCh">
    <p id="Взрослые">Взрослые              
    <button type="button"  onclick="this.nextElementSibling.stepDown()">-</button>
    <input type="number"  min="1" max="30"value="2" readonly class="raz">
    <button type="button"  onclick="this.previousElementSibling.stepUp()">+</button>
    </p>
    <p id="Дети">Дети                       
    <button type="button"  onclick="this.nextElementSibling.stepDown()">-</button>
    <input type="number"  min="0" max="10" value="0" readonly class="raz">
    <button type="button"  onclick="this.previousElementSibling.stepUp()">+</button>
    </p>
    <p id="Номера">Номера                  
    <button type="button"  onclick="this.nextElementSibling.stepDown()">-</button>
    <input type="number"  min="1" max="30" value="1" readonly class="raz">
    <button type="button"  onclick="this.previousElementSibling.stepUp()">+</button>
    </p>
    </div>
    </div>
    </div>
</template>
<script>

</script>
<style>
input[type='checkbox']
{
display:none;
}
.popup{
position: absolute;
top: 300px;
left: 600px;
margin:auto;
display:none;
width: 350px;
height: 180px;
background: #fffafa;
border-radius:4px;
box-shadow:-13px 15px 58px 7px rgba(5,5,5,0.38);
-webkit-box-shadow:-13px 15px 58px 7px rgba(5,5,5,0.38);
-moz-box-shadow:-13px 15px 58px 7px rgba(5,5,5,0.38);
}
#textCh{
position:absolute;
left: 20px;
font-weight: bold;
}
#Дети{
position:absolute;
top:55px;
}
#Номера{
position:absolute;
top:110px;
}

#Cus{
position: absolute;
top: 240px;
left: 660px;
 font-size: 16px;
 font-weight: bold;
 color: rgb(68,68,68);
height:51px;
width:250px;
 border: 1px solid rgba(0,0,0,.1);
 border-radius: 3px;
 background: rgb(245,245,245) linear-gradient(#f4f4f4, #f1f1f1);
   transition: all .218s ease 0s;
  z-index: 1;
}
#Cus:hover {
color: rgb(24,24,24);
  border: 1px solid rgb(198,198,198);
  background: #f7f7f7 linear-gradient(#f7f7f7, #f1f1f1);
  box-shadow: 0 1px 2px rgba(0,0,0,.1);
}
#Cus:active {
color: rgb(51,51,51);
border: 1px solid rgb(204,204,204);
background: rgb(238,238,238) linear-gradient(rgb(238,238,238), rgb(224,224,224));
box-shadow: 0 1px 2px rgba(0,0,0,.1) inset;
}
input:checked ~ .popup{
display: block;
}
.raz {
  all: unset;
  -moz-appearance: textfield;
  width: 3em;
  text-align: center;
}
.raz::-webkit-inner-spin-button {
  display: none;
}



</style>
