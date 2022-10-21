<template>
  <div class="left-side-menu-wrapper">
    <div class="left-side-menu">
      <div class="left-side-menu__menu-button">
        <div class="left-side-menu__menu-button-line left-side-menu__menu-button-line-1"></div>
        <div class="left-side-menu__menu-button-line left-side-menu__menu-button-line-2"></div>
        <div class="left-side-menu__menu-button-line left-side-menu__menu-button-line-3"></div>
      </div>
      <vertical-menu/>
      <left-side-menu-down-scroll/>
    </div>
  </div>
</template>

<script>
import VerticalMenu from '@/components/VerticalMenu.vue';
import LeftSideMenuDownScroll from '@/components/LeftSideMenuDownScroll.vue';

export default {
  name: 'LeftSideMenu',
  
  components: {
    VerticalMenu,
    LeftSideMenuDownScroll,
  },
}
</script>

<style scoped>
.left-side-menu-wrapper {
  display: flex;
  flex-direction: column;
  justify-content: center;
}
.left-side-menu {
  z-index: 4;
  margin-left: 36px;
}
.left-side-menu__menu-button {
  position: absolute;
  top: 37.5px;

  width: 19px;
  height: 16px;
}
.left-side-menu__menu-button:hover {
  cursor: pointer;
}
.left-side-menu__menu-button-line {  
  position: absolute;

  width: 18.6px;
  height: 1px;

  border: 1px solid #333333;
}
.left-side-menu__menu-button-line-1 {
  top: 0;
  left: 0;
}
.left-side-menu__menu-button-line-2 {
  top: 8px;
  left: 0;
}
.left-side-menu__menu-button-line-3 {
  top: 16px;
  left: 0;
}
</style>
