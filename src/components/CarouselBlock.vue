<template>
  <div class="carousel-wrapper">
    <div class="carousel">
      <div class="carousel__number">
        {{ normalizedActiveSlideIndex }}/8
      </div>
      <div
        class="carousel__next-slide"
        @click="next"
      >
        <img src="@/assets/images/Arrow-right.png">
      </div>
      <div
        class="carousel__prev-slide"
        @click="prev"
      >
        <img src="@/assets/images/Arrow-left.png">
      </div>
      <div class="carousel__image">
        <img :src="activeSlide.src"/>
      </div>
      <div
        class="carousel__text"
      >
        {{ activeSlide.text }}
      </div>
    </div>
  </div>
</template>

<script>
import slides from '@/data/slides';

export default {
  name: 'CarouselBlock',
  data() {
    return {
      slides,
      activeSlideIndex: 0,
    };
  },
  methods: {
    prev() {
      if (this.activeSlideIndex === 0) return;
      this.activeSlideIndex -= 1;
    },
    next() {
      if (this.activeSlideIndex === 7) return;
      this.activeSlideIndex += 1;
    }
  },
  computed: {
    activeSlide() {
        return this.slides[this.activeSlideIndex];
    },
    normalizedActiveSlideIndex() {
      return this.activeSlideIndex + 1;
    }
  },
}
</script>

<style scoped>
.carousel {
  display: flex;
  justify-content: center;

  width: 900px;
}
.carousel-wrapper {
  display: flex;
  justify-content: center;
}
.carousel__number {
  position: absolute;
  top: 176px;

  display: flex;
  align-items: center;
  justify-content: center;

  width: 56px;
  height: 56px;

  border-radius: 50px;

  user-select: none;

  background: #FFFFFF;
  box-shadow: 0px 5px 26px rgba(0, 0, 0, 0.1);

  font-family: 'Kinopoisk';
  font-weight: 700;
  font-size: 15px;
  line-height: 18px;
}
.carousel__image {
  position: absolute;
  top: 40%;

  z-index: 1;

  width: 303.13px;
  height: 436px;

  user-select: none;
}
.carousel__text {
  position: absolute;
  bottom: 20%;

  z-index: 4;

  width: 900px;
  max-width: 60%;
  
  text-align: center;
  letter-spacing: 0.4px;

  font-family: 'Kinopoisk';
  font-weight: 300;
  font-size: 20px;
  line-height: 32px;

  color: #000000;
}
.carousel__next-slide {
  position: absolute;
  right: 220px;
  top: 50%;

  z-index: 3;

  display: flex;
  justify-content: center;
  align-items: center;
  
  width: 40px;
  height: 40px;

  border: 1px solid #333333;
  border-radius: 50px;

  user-select: none;
}
.carousel__next-slide:hover {
  cursor: pointer;
}
.carousel__next-slide img {
  width: 15px;
  height: 4px;
}
.carousel__prev-slide {
  position: absolute;
  left: 220px;
  top: 50%;

  z-index: 3;

  display: flex;
  justify-content: center;
  align-items: center;

  height: 40px;
  width: 40px;

  border: 1px solid #333333;
  border-radius: 50px;

  user-select: none;
}
.carousel__prev-slide:hover {
  cursor: pointer;
}
.carousel__prev-slide img {
  width: 15px;
  height: 4px;
}

@media screen and (max-width: 899px) {
.carousel__text {
  position: absolute;
  bottom: 15%;
  font-size: 18px;
  line-height: 30px;
}
}

</style>
