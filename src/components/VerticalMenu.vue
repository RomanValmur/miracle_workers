<template>
  <div class="vertical-menu">
    <div class="vertical-menu__line vertical-menu__item-disactive vertical-menu__item-1"></div>
    <div class="vertical-menu__line vertical-menu__item-adjust vertical-menu__item-2"></div>
    <div class="vertical-menu__item-active vertical-menu__item-3">
        <span>03</span>Подсказки
        <div class="vertical-menu__line-active"></div>
    </div>
    <div class="vertical-menu__line vertical-menu__item-adjust vertical-menu__item-4"></div>
  </div>
</template>

<script>
export default {
  name: 'VerticalMenu',
}
</script>

<style scoped>
.vertical-menu__line-active {
  position: absolute;
  top: 20px;

  width: 132px;
  
  border: 1px solid #333333;
}
.vertical-menu__line {
  position: absolute;
  border: 1px solid #333333;
}
.vertical-menu__item-disactive {
  width: 4px;
}
.vertical-menu__item-adjust {
  width: 8px;
}
.vertical-menu__item-1 {
  top: 0;
}
.vertical-menu__item-2 {
  top: 50px;
}
.vertical-menu__item-3 {
  top: 80px;
}
.vertical-menu__item-4 {
  top: 150px;
}
.vertical-menu__item-active {
  position: absolute;

  font-family: 'Kinopoisk';
  font-size: 16px;
  line-height: 15px;
}
.vertical-menu__item-active span {
  margin-right: 30px;

  font-weight: 700;
}
.vertical-menu {
  position: absolute;
  top: calc(50% - 160px/2);
  
  width: 152px;
  height: 159.53px;
}
</style>
