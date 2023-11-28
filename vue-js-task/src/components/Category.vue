<template>
  <div class="collection_list">
    <div class="collection_list_wrapper">
      <div class="collection_list_cards">
        <div class="card_list">
          <div v-for="(item, index) in items" :key="{ index }">
            <a>
              <div class="collection_card">
                <div class="product_img">
                  <img :src="item.image" />
                  <p class="product_name">{{ item.name }}</p>
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
  name: 'CategoryNew',
  props: ['items'],
};
</script>

<style scoped>
.product_img{
  position: relative;
}
.product_name{
  position: absolute;
  bottom: 0px;
  backdrop-filter: blur(20px);
  background: rgba(255, 255, 255, 0.349);
  padding: 20px 0px;
  margin: 0px;
  font-family: "Playfair Display";
  color: white;
  font-size: 20px;
  width: 100%;
  display: flex;
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
  list-style: none;
  grid-template-columns: repeat(3,1fr);
  gap:20px
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
