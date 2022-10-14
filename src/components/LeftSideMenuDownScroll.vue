<template>
  <div class="down-scroll">
    <img src="@/assets/images/Arrow-scroll-down.png" width="65px"/>
    <span>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;Скорольте вниз</span>
  </div>
</template>

<script>
export default {
  name: 'LeftSideMenuDownScroll',
}
</script>

<style scoped>
.down-scroll {
  position: absolute;
  left: -60px;
  bottom: 120px;

  display: flex;

  width: 201px;
  height: 22px;

  align-items: center;
  
  transform: rotate(-90deg);
}
.down-scroll span {
  height: 21px;

  font-family: 'Kinopoisk';
  font-size: 14px;
  line-height: 15px;

  color: #333333;
}
.down-scroll img {
  height: 5px;
  opacity: 0.7;
}
</style>
