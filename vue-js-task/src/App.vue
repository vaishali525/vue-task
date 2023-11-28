<template>
  <div id="app">
    

    <HeaderData/>
    <HeroBanner/>
    <MIniCard/>
    <CollectionList :title="'Trending T-Shirts'" :items="first"/>
    <CollectionList :title="'Featured Products'" :items="second"/>
    <img src="/assets/banner1 2.png" style="width: 100%;"/>
    <CollectionList :title="'New Products'" :items="second"/>
    <CollectionList :title="'Best Selling Products'" :items="second"/>
    <Category :items="third"/>
    <img src="/assets/banner1 3.png" style="width: 100%;"/>
    <Discount :items="four"/>

    <FooterNew />
  </div>
</template>

<script>

import HeaderData from './components/HeaderData.vue'
import HeroBanner from './components/HeroBanner.vue';

import 'bootstrap/dist/css/bootstrap.css';
import MIniCard from './components/MIniCard.vue';
import CollectionList from './components/CollectionList.vue';
import Category from './components/Category.vue';
import Discount from './components/Discount.vue';
import FooterNew from './components/FooterNew.vue';

export default {
  name: 'App',
  components: {
    HeaderData,
    HeroBanner,
    MIniCard,
    CollectionList,
    Category,
    FooterNew,
    Discount
  },
  data() {
    return { 
      first: [
      {image:"/assets/Rectangle 3.png",name:"Men Henley Neck Full Sleeve Red Wine",sellingprice:399,price:1299,size:['s','m',"l","xl","xll"]},
      {image:"/assets/Rectangle 4.png",name:"Men Henley Neck Full Sleeve Red Wine",sellingprice:399,price:1299,size:['s','m',"l","xl","xll"]},
      {image:"/assets/Rectangle 5.png",name:"Men Henley Neck Full Sleeve Red Wine",sellingprice:399,price:1299,size:['s','m',"l","xl","xll"]},
      {image:"/assets/Rectangle 6.png",name:"Men Henley Neck Full Sleeve Red Wine",sellingprice:399,price:1299,size:['s','m',"l","xl","xll"]},
      {image:"/assets/Rectangle 3.png",name:"Men Henley Neck Full Sleeve Red Wine",sellingprice:399,price:1299,size:['s','m',"l","xl","xll"]},
      {image:"/assets/Rectangle 4.png",name:"Men Henley Neck Full Sleeve Red Wine",sellingprice:399,price:1299,size:['s','m',"l","xl","xll"]},
      {image:"/assets/Rectangle 5.png",name:"Men Henley Neck Full Sleeve Red Wine",sellingprice:399,price:1299,size:['s','m',"l","xl","xll"]},
      {image:"/assets/Rectangle 6.png",name:"Men Henley Neck Full Sleeve Red Wine",sellingprice:399,price:1299,size:['s','m',"l","xl","xll"]},
      ],
      second: [
      {image:"/assets/Rectangle 3.png",name:"Men Henley Neck Full Sleeve Red Wine",sellingprice:399,price:1299,size:['s','m',"l","xl","xll"]},
      {image:"/assets/Rectangle 4.png",name:"Men Henley Neck Full Sleeve Red Wine",sellingprice:399,price:1299,size:['s','m',"l","xl","xll"]},
      {image:"/assets/Rectangle 5.png",name:"Men Henley Neck Full Sleeve Red Wine",sellingprice:399,price:1299,size:['s','m',"l","xl","xll"]},
      {image:"/assets/Rectangle 6.png",name:"Men Henley Neck Full Sleeve Red Wine",sellingprice:399,price:1299,size:['s','m',"l","xl","xll"]},
      ],
      third: [
      {image:"/assets/c1.png",name:"Streetwear Collections",sellingprice:399,price:1299,size:['s','m',"l","xl","xll"]},
      {image:"/assets/c2.png",name:"Striped T-Shirts",sellingprice:399,price:1299,size:['s','m',"l","xl","xll"]},
      {image:"/assets/c3.png",name:"Round Neck T-Shirts",sellingprice:399,price:1299,size:['s','m',"l","xl","xll"]},
      {image:"/assets/c6.png",name:"Printed T-Shirts",sellingprice:399,price:1299,size:['s','m',"l","xl","xll"]},
      {image:"/assets/c5.png",name:"Oversized T-Shirts",sellingprice:399,price:1299,size:['s','m',"l","xl","xll"]},
      {image:"/assets/c4.png",name:"Half Sleeves T-Shirts",sellingprice:399,price:1299,size:['s','m',"l","xl","xll"]},
      ],
      four: [
      {image:"/assets/diamond 1.png",color:"#CCCEA7",discount:85},
      {image:"/assets/discount 1.png",color:"#D6BEBE",discount:75},
      ],
   }
  },

}
</script>

<style>
  @import url('https://fonts.googleapis.com/css2?family=Playfair+Display&display=swap');
#app {
  font-family: Montserrat;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
}
*{
  margin: 0;
  padding: 0;
}

</style>
