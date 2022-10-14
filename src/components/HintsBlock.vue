<template>
<div class="hints">
  <hints-overlay/>
  <kinopoisk-logo/>
  <hints-title/>
  <carousel-block/>
  <find-promo-button/>
  <left-side-menu/>
  <right-side-menu/>
</div>
</template>

<script>
import HintsOverlay from '@/components/HintsOverlay.vue';
import KinopoiskLogo from '@/components/KinopoiskLogo.vue';
import HintsTitle from '@/components/HintsTitle.vue';
import CarouselBlock from '@/components/CarouselBlock.vue';
import FindPromoButton from '@/components/FindPromoButton.vue';
import LeftSideMenu from '@/components/LeftSideMenu.vue';
import RightSideMenu from '@/components/RightSideMenu.vue';

export default {
  name: 'HintsBlock',
  components: {
    HintsOverlay,
    KinopoiskLogo,
    HintsTitle,
    CarouselBlock,
    FindPromoButton,
    LeftSideMenu,
    RightSideMenu,
  },
}
</script>

<style scoped>
.hints {
  position: absolute;
  top: 0;
  left: 0;

  z-index: 1;
  
  overflow: hidden;

  background-position: center;
  background-repeat: no-repeat;
  background-size: cover;
  background-image: url(@/assets/images/Back1.png);
}

@media screen and (min-width: 900px) and (min-height: 700px) {
  .hints {
    width: 100vw;
    height: 100vh;
}
}

@media screen and (min-width: 900px) and (max-height: 699px) {
  .hints {
    width: 100vw;
    height: 700px;
}
}

@media screen and (max-width: 899px) {
  .hints {
    width: 900px;
    height: 700px;
}
}

</style>
