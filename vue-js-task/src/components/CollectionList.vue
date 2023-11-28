<template>
  <div class="collection_list">
    <div class="collection_list_wrapper">
      <h2 class="hr_line"><span>{{ title }}</span></h2>
      <div class="collection_list_cards">
        <div class="card_list">
          <div v-for="(item, index) in items" :key="{ index }">
            <a>
              <div class="collection_card">
                <div class="product_img">
                  <img :src="item.image" />
                </div>
                <div class="product_desc">
                  <p class="product_name">{{ item.name }}</p>
                  <p class="product_price">₹{{ item.sellingprice }}<span class="orignal_price"> ₹{{ item.price }}</span></p>
                </div>
              </div>
              <div class="size">
                    <div v-for="(val, index1) in item.size" :key="{ index1 }"><span>{{ val }}</span></div>
                  </div>
            </a>
          </div>
        </div>
        <div class="view_all">
              <button>View all</button>
          </div>
      </div>
    </div>
  </div>
</template>
<script>
export default {
  name: "CollectionList",
  props: ["title", "items"],
};
</script>

<style scoped>
.orignal_price{
  color: #FF0000;
  text-decoration: line-through;
  font-size: 14px;
  font-weight: 400;
}
.size{
  display: flex;
  width: 100%;
  justify-content: space-evenly;
}
.size div{
  font-weight: 500;
  text-transform: uppercase;
  font-family: 'Montserrat';
  font-size: 16px;
  text-align: center;
  display: grid;
  place-items: center;
  width: 40px;
  border: 1px solid #E6E6E6;
  height: 40px;
}
h2 {
   width: 100%; 
   text-align: center; 
   border-bottom: 1px solid #FFC7D1; 
   line-height: 0.1em;
   margin: 10px 0 20px; 
} 

h2 span { 
    background:#ffffff; 
    padding:0 10px; 
}
.view_all{
  width: 100%;
  display: grid;
  margin: 25px 0px;
  place-items: center;
}
.view_all button{
  border: none;
  padding: 20px;
  outline: none;
  background: #770015;
  color: white;
  font-weight: 500;
  text-transform: uppercase;
  font-family: 'Montserrat';
  font-size: 16px;
}
.collection_list {
  max-width: 1120px;
  margin: 0 auto;
}
.collection_list_wrapper {
  margin-top: 68px;
}
.collection_list_wrapper h1 {
  font-family: "Playfair Display";
  font-size: 36px;
  font-weight: 600;
  text-align: center;
  line-height: 47.99px;
  margin: 0;
}
.collection_list_cards {
  margin: 48px 0;
  display: flex;
  flex-direction: column;
  align-items: center;
  /* justify-content: center; */
}
.card_list {
  /* display: flex;
  gap: 23.3px; */
  display: grid;
  list-style: none;
  grid-template-columns: repeat(4,1fr);
  gap:21px
}
.collection_card {
  display: flex;
  flex-direction: column;
  align-items: center;
  gap: 10px;
}
.product_desc {
  display: flex;
  flex-direction: column;
  gap: 10px;
}
.product_desc .product_name {
  max-width: 147px;
  margin: 0 auto;
  font-size: 14px;
  font-weight: 400;
  text-align: center;
  line-height: 17.07px;
}
.product_price {
  font-size: 18px;
  font-weight: 700;
  padding: 0;
  margin: 0;
  text-align: center;
}
</style>
