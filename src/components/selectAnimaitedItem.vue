<template>
  <div class="d-flex mt-2">
    <div class="item-selected w-50">
      <div class="selected-item w-100" v-if="activeIndex === 1">
        <img :style="style3d" src="https://cdn.prod.website-files.com/63d3e96d846e7c323c1bed54/652807b1069d5a80c3a6202a_reciever-slide-01-card.webp" class="first-img">
        <img :style="style3d" src="https://w230203-807.webasyst.cloud/wa-data/public/blog/img/dae02389b6d789343c26b6ccb9d41f9a.jpg" class="second-img">
      </div>
      <div class="selected-item w-100" v-if="activeIndex === 2">
        <img :style="style3d" src="https://cdn.prod.website-files.com/63d3e96d846e7c323c1bed54/652807b1069d5a80c3a6202a_reciever-slide-01-card.webp" class="first-img">
        <img :style="style3d" src="https://w230203-807.webasyst.cloud/wa-data/public/blog/img/dae02389b6d789343c26b6ccb9d41f9a.jpg" class="second-img">
      </div>
      <div class="selected-item w-100" v-if="activeIndex === 3">
        <img :style="style3d" src="https://cdn.prod.website-files.com/63d3e96d846e7c323c1bed54/652807b1069d5a80c3a6202a_reciever-slide-01-card.webp" class="first-img">
        <img :style="style3d" src="https://cdn.prod.website-files.com/63d3e96d846e7c323c1bed54/652807b051fe23bb1913e1ee_reciever-slide-02-tim.webp" class="second-img">
      </div>
    </div>
    <div class="item-select w-50">
      <div class="select-item" :class="{ 'active': activeIndex === 1 }" @click="setActive(1)">
        <div class="item-title">
          Почему мы
        </div>
        <div class="item-description">
          Мы предоставляем услуги распила и кромления ЛДСП, МДФ и других материалов. Изготавливаем мебель на заказ с учетом ваших предпочтений и особенностей интерьера. Гарантируем высокое качество работы, точность и доступные сроки выполнения.
        </div>
      </div>
      <div class="select-item" :class="{ 'active': activeIndex === 2 }" @click="setActive(2)">
        <div class="item-title">
          Качество, стиль и точность в каждом проекте
        </div>
        <div class="item-description">
          Осуществляем доставку готовых деталей и сборку мебели на месте. Работаем как с частными заказами, так и с крупными проектами для бизнеса.
        </div>
      </div>
      <div class="select-item" :class="{ 'active': activeIndex === 3 }" @click="setActive(3)">
        <div class="item-title">
          Гибкость
        </div>
        <div class="item-description">
          Предлагаем гибкие условия сотрудничества, включая выбор материалов, сроки выполнения и бюджет.
        </div>
      </div>
    </div>
  </div>
</template>

<script setup lang="ts">
import { ref, onMounted } from 'vue'
import type { Ref } from 'vue'

const style3d: Ref<string> = ref('transform: translate3d(0px, 0px, 0px) scale3d(0, 0, 0) rotateX(0deg) rotateY(0deg) rotateZ(0deg) skew(0deg, 0deg);')
const activeIndex: Ref<number> = ref(1);

function setActive (index: number) {
  style3d.value = 'transform: translate3d(0px, 0px, 0px) scale3d(0, 0, 0) rotateX(0deg) rotateY(0deg) rotateZ(0deg) skew(0deg, 0deg);'
  activeIndex.value = index;

  setTimeout(() => {
    style3d.value = 'transform: translate3d(0px, 0px, 0px) scale3d(1, 1, 1) rotateX(0deg) rotateY(0deg) rotateZ(0deg) skew(0deg, 0deg);'
  }, 100);
}

onMounted(() => {
  setTimeout(() => {
    style3d.value = 'transform: translate3d(0px, 0px, 0px) scale3d(1, 1, 1) rotateX(0deg) rotateY(0deg) rotateZ(0deg) skew(0deg, 0deg);'
  }, 100);
})


</script>

<style scoped>

.first-img {
  width: 50%;
  margin-bottom: 10px;
  position: absolute;
  top: 20px;
  left: 20px;
  z-index: 100;
  transition: all 0.2s ease-in-out;
}

.second-img {
  width: 40%;
  margin-bottom: 10px;
  position: absolute;
  right: 20px;
  top: 215px;
  border-radius: 20px;
  transition: all 0.2s ease-in-out;
}

.item-select {
  display: flex;
  flex-direction: column;
  justify-content: center;
}

.select-item {
  cursor: pointer;
  margin: 20px;
  padding: 20px;
  transition: all 0.2s ease-in-out;
}

.item-title {
  font-weight: bold;
  font-size: 20px;
}

.select-item:hover {
  background: #606C38;
  color: #fff;
  transform: scale(1.05);
}

.select-item.active {
  background: #606C38;
  color: #fff;
}

.selected-item {
  justify-content: space-between;
  position: relative;
  display: flex;
  flex-wrap: wrap;
}

.item-selected {
  position: relative;
}

</style>
