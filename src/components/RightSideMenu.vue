<template>
  <div class="right-side-menu">
    <a href="#">hd.kinopoisk.ru</a>
  </div>
</template>

<script>
export default {
  name: 'RightSideMenu',
}
</script>

<style scoped>
.right-side-menu {
  position: absolute;
  top: calc(50% - 30.79px/2);
  right: 30px;
  
  z-index: 4;

  display: flex;
  align-items: center;

  height: 30px;

  font-family: 'Kinopoisk';
  font-size: 14px;
  line-height: 15px;

  text-align: center;

  transform: rotate(90deg);
}
.right-side-menu a {
  color: #333333;
  text-decoration: none;
}
</style>
  