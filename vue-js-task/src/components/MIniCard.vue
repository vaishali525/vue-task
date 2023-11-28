<template>
  <div class="mini_card">
    <div class="mini_card_wrap1">
      <div>
        <a><img src="../assets/image 2.png" /></a>
      </div>
      <div>
        <a><img src="../assets/image 3.png" /></a>
      </div>
    </div>
    <div class="mini_card_wrap2">
      <div>
        <a><img src="../assets/image 4.png" /></a>
      </div>
      <div>
        <a><img src="../assets/image 5.png" /></a>
      </div>
      <div>
        <a><img src="../assets/image 6.png" /></a>
      </div>
    </div>
  </div>
</template>
<script>
export default {
  name: "MiniCard",
};
</script>
<style>
.mini_card {
  max-width: 1120px;
  margin: 0 auto;
}
.mini_card_wrap1 {
  gap: 20px;
  display: flex;
  margin-top: 68px;
}
.mini_card_wrap2 {
    margin-top: 16px;
  gap: 20px;
  display: flex;
}
</style>
