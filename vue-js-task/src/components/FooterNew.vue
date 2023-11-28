<template>
  <div class="footer">
    <div class="collection_list">
      <div class="gridbox">
        <div>
          <div>Lorem Ipsum is simply dummy text of the printing and typesetting industry. Lorem Ipsum has been the industry's standard dummy text ever since the 1500s, when an unknown printer took a galley of type and scrambled it to make a type specimen book. It has survived not only five centuries....</div>
          <div class="flex"><img v-for="(item, index) in [1,2,3,4,5]" :key="{ index }" :src="'/assets/i'+item+'.png'"/></div>
        </div>
        <div class="menu">
          <h2 class="title">ONLINE SHOPPING</h2>
          <p>Men’s T-Shirts</p>
          <p>Women’s Wear</p>
          <p>Winter Collections</p>
          <p>Hooded T-Shirts</p>
          <p>Streetwear Collections</p>
        </div>
        <div class="menu">
          <h2 class="title">CUSTOMER POLICIES</h2>
          <p>About Us</p>
          <p>Terms & Conditions</p>
          <p>Shipping & Returns Policy</p>
          <p>Cancellation & Refund Policy</p>
          <p>Contact Us</p>
        </div>
        <div class="menu">
          <h2 class="title">STORE INFORMATION</h2>
          <p>
            <span>
              <svg
                width="24"
                height="25"
                viewBox="0 0 24 25"
                fill="none"
                xmlns="http://www.w3.org/2000/svg"
              >
                <path
                  d="M20 10.876C20 15.294 12 22.876 12 22.876C12 22.876 4 15.294 4 10.876C4 8.75424 4.84285 6.71941 6.34315 5.21912C7.84344 3.71883 9.87827 2.87598 12 2.87598C14.1217 2.87598 16.1566 3.71883 17.6569 5.21912C19.1571 6.71941 20 8.75424 20 10.876Z"
                  stroke="#1C1C1C"
                  stroke-width="1.5"
                />
                <path
                  d="M12 11.876C12.2652 11.876 12.5196 11.7706 12.7071 11.5831C12.8946 11.3955 13 11.1412 13 10.876C13 10.6108 12.8946 10.3564 12.7071 10.1689C12.5196 9.98133 12.2652 9.87598 12 9.87598C11.7348 9.87598 11.4804 9.98133 11.2929 10.1689C11.1054 10.3564 11 10.6108 11 10.876C11 11.1412 11.1054 11.3955 11.2929 11.5831C11.4804 11.7706 11.7348 11.876 12 11.876Z"
                  fill="#1C1C1C"
                  stroke="#1C1C1C"
                  stroke-width="1.5"
                  stroke-linecap="round"
                  stroke-linejoin="round"
                />
              </svg> </span
            ><span
              >Lorem Ipsum is simply dummy text of the printing and typesetting
              industry.
            </span>
          </p>
          <p>
            <span
              ><svg
                width="24"
                height="25"
                viewBox="0 0 24 25"
                fill="none"
                xmlns="http://www.w3.org/2000/svg"
              >
                <path
                  d="M18.118 15.578L14 16.376C11.218 14.98 9.49999 13.376 8.49999 10.876L9.26999 6.74598L7.81499 2.87598H4.06399C2.93599 2.87598 2.04799 3.80798 2.21699 4.92298C2.63699 7.70598 3.87699 12.753 7.49999 16.376C11.305 20.181 16.786 21.832 19.802 22.489C20.967 22.742 22 21.834 22 20.641V17.057L18.118 15.578Z"
                  stroke="#1C1C1C"
                  stroke-width="1.5"
                  stroke-linecap="round"
                  stroke-linejoin="round"
                />
              </svg> </span
            ><span>Call Us: 1234567890 </span>
          </p>
          <p>
            <span
              ><svg
                width="24"
                height="25"
                viewBox="0 0 24 25"
                fill="none"
                xmlns="http://www.w3.org/2000/svg"
              >
                <path
                  d="M7 9.87598L12 13.376L17 9.87598"
                  stroke="#1C1C1C"
                  stroke-width="1.5"
                  stroke-linecap="round"
                  stroke-linejoin="round"
                />
                <path
                  d="M2 17.876V7.87598C2 7.34554 2.21071 6.83684 2.58579 6.46176C2.96086 6.08669 3.46957 5.87598 4 5.87598H20C20.5304 5.87598 21.0391 6.08669 21.4142 6.46176C21.7893 6.83684 22 7.34554 22 7.87598V17.876C22 18.4064 21.7893 18.9151 21.4142 19.2902C21.0391 19.6653 20.5304 19.876 20 19.876H4C3.46957 19.876 2.96086 19.6653 2.58579 19.2902C2.21071 18.9151 2 18.4064 2 17.876Z"
                  stroke="#1C1C1C"
                  stroke-width="1.5"
                />
              </svg> </span
            ><span>Email Us: info@yourmail.com </span>
          </p>
        </div>
      </div>
    </div>
    <div class="bottom_footer">©2022-23 Powered By dummy team</div>
  </div>
</template>
<script>
export default {
  name: "FooterNew",
};
</script>

<style scoped>
.flex{
  display: flex;
  gap: 5px;
}
.menu p{
  margin: 0;
  padding: 10px 0px;
  font-weight: 500;
  font-size: 14px;
  color: #1C1C1C;
  font-family: "Montserrat";
}
.title{
  color: #770015;
  font-size: 18px;
  font-weight: 600;
  font-family: "Playfair Display";
  margin-bottom: 20px;
}
.gridbox {
  display: grid;
  grid-template-columns: 30% 23% 23% 23%;
}
.footer {
  display: flex;
  justify-content: center;
  align-items: center;
  flex-direction: column;
}
.collection_list {
  max-width: 1120px;
  margin: 0 auto;
}
.bottom_footer {
  display: flex;
  width: 100%;
  color: white;
  padding: 15px 0px;
  justify-content: center;
  background: #000;
}
</style>
