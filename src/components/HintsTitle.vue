<template>
  <div class="hints__title">
    <h1>
      ОНИ ДОЛЖНЫ ЧТО-ТО ЗНАТЬ
    </h1>
  </div>
</template>

<script>
export default {
  name: 'HintsTitle',
}
</script>

<style scoped>
.hints__title {
  display: flex;
  justify-content: center;
  user-select: none;
}
.hints__title h1 {
  position: absolute;
  top: 70px;

  margin: 0;

  width: 790px;
  height: 72px;

  text-align: center;
  letter-spacing: -0.692308px;
  text-transform: uppercase;

  font-family: 'Futura';
  font-style: normal;
  font-weight: bold;
  font-size: 45px;
  line-height: 72px;

  color: #FFCC64;
}

@media screen and (min-width: 900px) and (max-width: 1024px) {
  .hints__title h1 {
    font-size: 35px;
  }
}

@media screen and (max-width: 899px) {
  .hints__title h1 {
    font-size: 25px;
  }
}

</style>
