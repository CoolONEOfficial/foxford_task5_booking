<template>
    <!--TODO: hotels slider-->
</template>

<script>
    export default {
        name: "HotelsSlider"
    }
</script>

<style scoped>
.frms{
  min-width: 800px;
}
.txtnn{
  position: relative;
  font-family: Segoe UI;
  font-size: 20px;
  text-align: left;
  left: 19%;
  margin-top: 20px;
  margin-bottom: 20px;
  width: 60%;
}
.scroll2{
 position: relative;
 line-height: 170px;
 padding: 0 50px;
}
.scroll2 input{
 display: none;
}
.scroll2 div{
 margin-left: auto;
 margin-right: auto;
 width: 70%;
 overflow: hidden;
 white-space: nowrap;
 font-size: 0;
 position: static;
}
.scroll2 img{
 cursor: pointer;
 position: relative;
 right: 0em;
 width: 23%;
 height: 100%;
 transition: .6s;
 padding-left: 2%;
}
.scroll2 label{
  text-shadow: black 1px 1px 0,  black -1px -1px 0, 
               black -1px 1px 0, black 1px -1px 0;
  color: #FFFFFF;
  opacity: 0.6;
  cursor: pointer;
  font-weight: bold;
  font-size: calc(3.5vw + 5px);
  z-index: 1000;
  position: absolute;
  padding-left: 61.2%;
  margin-top: -14%;
  padding-top: calc(20% - 60px);
  width: calc(13% - 20px);
  margin-left: auto;
  margin-right: auto;
  right: calc(13% - 5px);
}
.scroll2 label:hover{
  opacity: 1;
}
.scroll2 input:nth-of-type(1):checked ~ label:nth-of-type(2):after,
.scroll2 input:nth-of-type(2):checked ~ label:nth-of-type(3):after{
 content: "\3009";
 position: absolute;
 right: 0;
}
.scroll2 input:nth-of-type(2):checked ~ label:nth-of-type(1):after,
.scroll2 input:nth-of-type(3):checked ~ label:nth-of-type(2):after{
 content: "\3008";
 position: absolute;
 left: 0;
}
.scroll2 input:nth-of-type(2):checked ~ div img {right: 25%;}
.scroll2 input:nth-of-type(3):checked ~ div img {right: 50%;}

</style>
<div class="frms">
  <div class="txtnn">Найдите идеальный дом или апартаменты для следующей поездки, куда бы вы ни отправились</div>
  <div class="scroll2">
    <input type="radio" id="40" name="rrrr" checked="checked"/>
    <input type="radio" id="41" name="rrrr"/>
    <input type="radio" id="42" name="rrrr"/>
    
    <label for="40"></label>
    <label for="41"></label>
    <label for="42"></label>
    <div>
<a href="https://www.booking.com/searchresults.html?aid=304142;label=gen173nr-1DCAEoggI46AdIM1gEaMIBiAEBmAEhuAEXyAEP2AED6AEBiAIBqAIDuAK305nnBcACAQ;sid=229a698ced18da069d5859f2ee832970;dest_id=-666610;dest_type=city;highlighted_hotels=913677;nflt=ht_id%3D212%3Bht_id%3D223%3Bht_id%3D213%3Bht_id%3D222%3Bht_id%3D232%3Bht_id%3D227%3Bht_id%3D228%3Bht_id%3D220%3Bht_id%3D219%3Bht_id%3D230%3Bht_id%3D214%3Bht_id%3D209%3Bht_id%3D201%3Bht_id%3D216%3Bht_id%3D215%3Bht_id%3D208%3Bht_id%3D224%3Bht_id%3D210%3Bht_id%3D229;bhc_from_index=1;bhc_from_index=1"><img src="https://i.ibb.co/CWBMkF7/1.png" alt=""/></a>
<a href="https://www.booking.com/searchresults.ru.html?label=gen173nr-1DCAEoggI46AdIM1gEaMIBiAEBmAEhuAEXyAEP2AED6AEBiAIBqAIDuAK305nnBcACAQ&sid=229a698ced18da069d5859f2ee832970&sb=1&src=index&src_elem=sb&error_url=https%3A%2F%2Fwww.booking.com%2Fbooking-home%2Findex.ru.html%3Flabel%3Dgen173nr-1DCAEoggI46AdIM1gEaMIBiAEBmAEhuAEXyAEP2AED6AEBiAIBqAIDuAK305nnBcACAQ%3Bsid%3D229a698ced18da069d5859f2ee832970%3Bsb_price_type%3Dtotal%26%3B&nflt=ht_id%253D201%253Bht_id%253D230%253Bht_id%253D232%253Bht_id%253D220%253Bht_id%253D219%253Bht_id%253D228%253Bht_id%253D229%253Bht_id%253D213&theme_id=74&theme_source=index&ss=%D0%98%D0%BC%D0%B5%D1%80%D0%BE%D0%B2%D0%B8%D0%B3%D0%BB%D0%B8%2C+%D0%9A%D0%B8%D0%BA%D0%BB%D0%B0%D0%B4%D1%8B%2C+Greece&is_ski_area=0&checkin_year=&checkin_month=&checkout_year=&checkout_month=&group_adults=2&group_children=0&b_h4u_keep_filters=&from_sf=1&ss_raw=%D0%B8%D0%BC%D0%B5%D1%80%D0%BE%D0%B2%D0%B8&ac_position=0&ac_langcode=ru&ac_click_type=b&dest_id=-818117&dest_type=city&place_id_lat=36.43256&place_id_lon=25.42283&search_pageview_id=68f847e7411f001c&search_selected=true"><img src="https://i.ibb.co/G0WPMvD/2.png" alt=""/></a>
  <a href="https://www.booking.com/searchresults.html?aid=304142;label=gen173nr-1DCAEoggI46AdIM1gEaMIBiAEBmAEhuAEXyAEP2AED6AEBiAIBqAIDuAK305nnBcACAQ;sid=229a698ced18da069d5859f2ee832970;dest_id=-2996338;dest_type=city;highlighted_hotels=1860177;nflt=ht_id%3D212%3Bht_id%3D223%3Bht_id%3D213%3Bht_id%3D222%3Bht_id%3D232%3Bht_id%3D227%3Bht_id%3D228%3Bht_id%3D220%3Bht_id%3D219%3Bht_id%3D230%3Bht_id%3D214%3Bht_id%3D209%3Bht_id%3D201%3Bht_id%3D216%3Bht_id%3D215%3Bht_id%3D208%3Bht_id%3D224%3Bht_id%3D210%3Bht_id%3D229;bhc_from_index=1;bhc_from_index=1"><img src="https://i.ibb.co/bBCrVLF/3.png" alt=""/></a>
  <a href="https://www.booking.com/searchresults.ru.html?label=gen173nr-1DCAEoggI46AdIM1gEaMIBiAEBmAEhuAEXyAEP2AED6AEBiAIBqAIDuAK305nnBcACAQ&sid=229a698ced18da069d5859f2ee832970&sb=1&src=index&src_elem=sb&error_url=https%3A%2F%2Fwww.booking.com%2Fbooking-home%2Findex.ru.html%3Flabel%3Dgen173nr-1DCAEoggI46AdIM1gEaMIBiAEBmAEhuAEXyAEP2AED6AEBiAIBqAIDuAK305nnBcACAQ%3Bsid%3D229a698ced18da069d5859f2ee832970%3Bsb_price_type%3Dtotal%26%3B&nflt=ht_id%253D201%253Bht_id%253D230%253Bht_id%253D232%253Bht_id%253D220%253Bht_id%253D219%253Bht_id%253D228%253Bht_id%253D229%253Bht_id%253D213&theme_id=74&theme_source=index&ss=%D0%A1%D0%BF%D0%BB%D0%B8%D1%82%2C+%D0%A1%D0%BF%D0%BB%D0%B8%D1%82%D1%81%D0%BA%D0%BE-%D0%94%D0%B0%D0%BB%D0%BC%D0%B0%D1%82%D0%B8%D0%BD%D1%81%D0%BA%D0%B0%D1%8F+%D0%B6%D1%83%D0%BF%D0%B0%D0%BD%D0%B8%D1%8F%2C+Croatia&is_ski_area=0&checkin_year=&checkin_month=&checkout_year=&checkout_month=&group_adults=2&group_children=0&b_h4u_keep_filters=&from_sf=1&ss_raw=%D1%81%D0%BF%D0%BB%D0%B8%D1%82&ac_position=0&ac_langcode=ru&ac_click_type=b&dest_id=-96492&dest_type=city&iata=SPU&place_id_lat=43.508583&place_id_lon=16.44075&search_pageview_id=68f847e7411f001c&search_selected=true"><img src="https://i.ibb.co/JtnpsGm/4.png" alt=""/></a>
  <a href="https://www.booking.com/searchresults.ru.html?label=gen173nr-1DCAEoggI46AdIM1gEaMIBiAEBmAEhuAEXyAEP2AED6AEBiAIBqAIDuAK305nnBcACAQ&sid=229a698ced18da069d5859f2ee832970&sb=1&src=index&src_elem=sb&error_url=https%3A%2F%2Fwww.booking.com%2Fbooking-home%2Findex.ru.html%3Flabel%3Dgen173nr-1DCAEoggI46AdIM1gEaMIBiAEBmAEhuAEXyAEP2AED6AEBiAIBqAIDuAK305nnBcACAQ%3Bsid%3D229a698ced18da069d5859f2ee832970%3Bsb_price_type%3Dtotal%26%3B&nflt=ht_id%253D201%253Bht_id%253D230%253Bht_id%253D232%253Bht_id%253D220%253Bht_id%253D219%253Bht_id%253D228%253Bht_id%253D229%253Bht_id%253D213&theme_id=74&theme_source=index&ss=%D0%9D%D0%B8%D1%86%D1%86%D0%B0%2C+%D0%9F%D1%80%D0%BE%D0%B2%D0%B0%D0%BD%D1%81+%E2%80%94+%D0%90%D0%BB%D1%8C%D0%BF%D1%8B+%E2%80%94+%D0%9B%D0%B0%D0%B7%D1%83%D1%80%D0%BD%D1%8B%D0%B9+%D0%91%D0%B5%D1%80%D0%B5%D0%B3%2C+France&is_ski_area=&checkin_year=&checkin_month=&checkout_year=&checkout_month=&group_adults=2&group_children=0&b_h4u_keep_filters=&from_sf=1&ss_raw=%D0%BD%D0%B8%D1%86%D1%86&ac_position=0&ac_langcode=ru&ac_click_type=b&dest_id=-1454990&dest_type=city&iata=NCE&place_id_lat=43.69808&place_id_lon=7.269624&search_pageview_id=68f847e7411f001c&search_selected=true&search_pageview_id=68f847e7411f001c&ac_suggestion_list_length=5&ac_suggestion_theme_list_length=0"><img src="https://i.ibb.co/CmrZxgp/5.png" alt=""/></a>
  <a href="https://www.booking.com/booking-home/index.ru.html?label=gen173nr-1DCAEoggI46AdIM1gEaMIBiAEBmAEhuAEXyAEP2AED6AEBiAIBqAIDuAK305nnBcACAQ;sid=229a698ced18da069d5859f2ee832970;bhc_from_index_bh=1"><img src="https://i.ibb.co/6DtdQCR/7.png" alt=""/></a>
    </div>
  </div>
</div>
