<template>
  <div class="logo">
    <img src="@/assets/images/KinoPoiskHDlogo.svg" alt="Логотип"/>
  </div>
</template>

<script>
export default {
  name: 'KinopoiskLogo',
}
</script>

<style scoped>
.logo {
  display: flex;
  justify-content: center;
  
  user-select: none;
}
.logo img {
  position: absolute;
  top: 21px;

  z-index: 4;
}
</style>
