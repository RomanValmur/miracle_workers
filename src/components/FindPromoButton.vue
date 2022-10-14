<template>
  <div class="find-promo-wrapper">
    <div class="find-promo">
      <span>Искать промокод&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;</span>
      <img src="@/assets/images/Arrow-right.png"/>
    </div>
  </div>
</template>

<script>
export default {
  name: 'FindPromoButton',
}
</script>

<style scoped>
.find-promo-wrapper {
  display: flex;
  justify-content: center;
}
.find-promo {
  position: absolute;
  bottom: 10%;

  z-index: 3;
  
  display: flex;
  align-items: center;

  border-radius: 8px;
  
  user-select: none;
}
.find-promo:hover {
  cursor: pointer;
}
.find-promo span {
  font-family: 'Kinopoisk';
  font-size: 15px;
  line-height: 18px;
  text-align: center;

  color: #333333;
}
.find-promo img {
  width: 26px;
  height: 5px;
}
</style>
