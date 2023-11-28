<template>
  <div class="header">
    <div class="top_header">
      <div class="anouncement_bar">
        <div class="left_bar">Welcome to Our Store Hiscraves</div>
        <div class="right_bar">
          <img src="../assets/Vector.svg" /><span
            >Call Us:<a>1234567890</a></span
          >
        </div>
      </div>
    </div>
    <div class="header_wrapper">
      <div class="header_nav">
        <a><img src="../assets/Group 3.svg" /></a>
      </div>
      <div class="header_logo">Logo Here</div>
      <div class="header_icon">
        <ul class="right_icon_menu">
          <li><a><img src="../assets/search.svg"/></a></li>
          <li><a><img src="../assets/wishlist.svg"/></a></li>
          <li><a><img src="../assets/cart.svg"/></a></li>
          <li><a><img src="../assets/login.svg"/></a></li>
        </ul>
      </div>
    </div>
  </div>
</template>
<script>
export default {
  name: "HeaderData",
  props: {
    msg: String,
  },
};
</script>
<style>
.header {
  width: 100%;
  display: block;
}
.top_header {
  background: #1f1f1f;
  line-height: 48px;
}
.anouncement_bar {
  max-width: 1120px;
  margin: 0 auto;
  width: 100%;
  display: flex;
  justify-content: space-between;
}
.left_bar {
  color: #ffffff;
  font-size: 14px;
}
.right_bar {
  color: #ffffff;
  font-size: 14px;
}
.header_wrapper {
  max-width: 1120px;
  margin: 0 auto;
  width: 100%;
  display: flex;
  justify-content: space-between;
  line-height: 88px;
}
ul.right_icon_menu {
    gap: 24px;
    list-style: none;
    display: inline-flex;
    margin: 0;
    padding: 0;
}
</style>
