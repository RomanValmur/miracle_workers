<template>
  <div class="hints__overlay"></div>
</template>

<script>
export default {
  name: 'HintsOverlay',
}
</script>

<style scoped>
.hints__overlay{
  position: absolute;
  top: 0;
  left: 0;
  
  z-index: 3;

  background-position: center;
  background-repeat: no-repeat;
  background-size: cover;
  background-image: url(@/assets/images/Back2.png);
}

@media screen and (min-width: 900px) and (min-height: 700px) {
  .hints__overlay {
    width: 100vw;
    height: 100vh;
}
}

@media screen and (min-width: 900px) and (max-height: 699px) {
  .hints__overlay {
    width: 100vw;
    height: 700px;
}
}

@media screen and (max-width: 899px) {
  .hints__overlay {
    width: 900px;
    height: 700px;
}
}

</style>
