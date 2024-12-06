<script setup lang="ts">
import { ref } from 'vue';

const slides = ref<string[]>([
  "https://www.igor-mann.ru/wp-content/uploads/2018/10/800h400-kartinka-dlya-bloga-27-2.jpg",
  "https://www.igor-mann.ru/wp-content/uploads/2019/02/800h400-kartinka-dlya-bloga-32-2.jpg",
  "https://www.igor-mann.ru/wp-content/uploads/2018/10/800h400-kartinka-dlya-bloga-30-3.jpg",
]);

const currentIndex = ref<number>(0);

const nextSlide = () => {
  currentIndex.value = (currentIndex.value + 1) % slides.value.length;
};

const prevSlide = () => {
  currentIndex.value =
    (currentIndex.value - 1 + slides.value.length) % slides.value.length;
};

//#606C38
</script>

<template>
  <div class="slider">
    <div
      class="slider-track"
      :style="{ transform: `translateX(-${currentIndex * 100}%)` }"
    >
<!--      <div class="slide" v-for="(slide, index) in slides" :key="index">-->
<!--        <img :src="slide" alt="Slide Image" />-->
<!--      </div>-->
      <div class="slide" :key="1">
        <img src='../assets/pexels-andreaedavis-27065116.jpg' alt="Slide Image" />
      </div>
      <div class="slide" :key="2">
        <img src='../assets/pexels-cristian-rojas-8447895.jpg' alt="Slide Image" />
      </div>
      <div class="slide" :key="3">
        <img src='../assets/pexels-curtis-adams-1694007-7601183.jpg' alt="Slide Image" />
      </div>
    </div>
    <button class="prev" @click="prevSlide">←</button>
    <button class="next" @click="nextSlide">→</button>
    <div class="indicator">
      <div
        v-for="(slide, index) in slides"
        :key="index"
        :class="['indicator-dot', { active: currentIndex === index }]"
        @click="currentIndex = index"
      ></div>
    </div>
  </div>
</template>

<style scoped>
.slider {
  position: relative;
  width: 100%;
  overflow: hidden;
  margin: 0 auto;
  height: 400px;
}

.slider-track {
  display: flex;
  transition: transform 0.5s ease-in-out;
}

.slide {
  min-width: 100%;
  box-sizing: border-box;
}

.slide img {
  display: block;
  width: 100%;
  height: auto;
}

button {
  position: absolute;
  top: 50%;
  transform: translateY(-50%);
  background-color: rgba(0, 0, 0, 0.5);
  color: white;
  border: none;
  padding: 10px 20px;
  cursor: pointer;
  font-weight: bold;
}

.prev {
  left: 10px;
}

.next {
  right: 10px;
}

.indicator {
  display: flex;
  justify-content: center;
  position: absolute;
  bottom: 10px;
  left: 50%;
  transform: translateX(-50%);
  gap: 10px;
  cursor: pointer;
}

.indicator-dot {
  width: 10px;
  height: 10px;
  border-radius: 50%;
  background-color: #687281;
  transition: background-color 0.3s ease;
}

.indicator-dot.active {
  background-color: #606C38;
}
</style>
