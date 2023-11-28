<template>
  <div class="collection_list">
    <div class="collection_list_wrapper">
      <div class="collection_list_cards">
        <div class="card_list">
          <div v-for="(item, index) in items" :key="{ index }" class="caty" :style="`background:`+item.color">
            <a>
              <div class="collection_card" >
                <div class="product_img">
                  <img :src="item.image" />
                  <p class="product_name_hurry">Hurry Up!</p>
                  <p class="product_name">{{ item.discount }}% OFF</p>
                  <p class="product_name_hurry">Sale</p>
                  <div class="view_all">
                      <button>Shop Now</button>
                  </div>
                </div>
              </div>
            </a>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>
<script>
export default {
  name: 'DiscountNew',
  props: ['items'],
};
</script>

<style scoped>
.view_all{
  width: 100%;
  display: grid;
  margin: 25px 0px;
  place-items: center;
}
.view_all button{
  border: none;
  padding: 10px 20px;
  border: 1px solid #fff;
  outline: none;
  background: #77001600;
  color: rgb(255, 255, 255);
  font-weight: 500;
  text-transform: uppercase;
  font-family: 'Montserrat';
  font-size: 16px;
}
.caty{
  padding: 50px 0px;
}
.product_img{
  display: grid;
  place-items: center;
}
.product_name{
  font-family: "Playfair Display";
  font-size: 84px;
  font-weight: 600;
  width: 100%;
  display: flex;
  align-items: center;
  justify-content: center;
}
.product_name_hurry{
  font-family: "Playfair Display";
  font-size: 36px;
  font-weight: 600;
  width: 100%;
  display: flex;
  margin: 20px 0px;
  align-items: center;
  justify-content: center;
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
  width: 100%;
  list-style: none;
  grid-template-columns: repeat(2,1fr);
  gap:30px
}
.collection_card {
  display: flex;
  flex-direction: column;
  align-items: center;
  justify-content: center;
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
