<template>
  <div class="homepage_section">
    <div class="hero_banner">
     <a><img src="../assets/image 1.png"/></a>
    </div>
    <div class="collection_card">
      <ul>
        <li><a><img src="../assets/Group 244 (1).png"/></a></li>
        <li><a><img src="../assets/Group 245 (1).png"/></a></li>
        <li><a><img src="../assets/Group 246 (1).png"/></a></li>
        <li><a><img src="../assets/Group 247.png"/></a></li>
        <li><a><img src="../assets/Group 248.png"/></a></li>
        <li><a><img src="../assets/Group 249.png"/></a></li>
      </ul>
    </div>
  </div>
</template>
<script>
export default {
  name: 'HeroBanner',
  props: {
    msg: String
  }
}
</script>
<style>
.hero_banner img{
  width: 100%;

}
.collection_card{
  max-width: 1120px;
  margin: 0 auto;
}
.collection_card ul{
  margin: 68px 0 0;
  padding: 0;
  display: flex;
  gap: 20px;
  list-style: none;
}
</style>