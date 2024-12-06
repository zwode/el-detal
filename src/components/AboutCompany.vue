<template>
  <div class="d-flex mt-2 justify-content-between flex-wrap">
    <div class="custom-block w-100 d-flex">
      <div class="custom-img w-50 mr-1">
        <img src="https://severplit.ru/thumb/2/pyK6LO3rn0yfaAhnxcVoXw/900r600/d/55112521_2.jpg"/>
      </div>
      <div class="custom-info w-50">
        <div class="custom-info-title mt-2">
          <div class="">
            Распил, кромление и мебель по индивидуальным заказам
          </div>
        </div>
        <div class="">
          <div class="custom-title">
            Мы предлагаем услуги распила и кромления ЛДСП, МДФ и других материалов с высокой точностью и качеством. Изготавливаем мебель по индивидуальным заказам: от корпусной мебели до встроенных решений. Наши специалисты помогут с проектированием, подбором материалов и фурнитуры. Используем современное оборудование, чтобы гарантировать надежность и долговечность изделий. Быстрые сроки выполнения и доступные цены – наш приоритет.
          </div>
        </div>
        <button class="custom-button">
          Рассчитать стоимость изготовления →
        </button>
      </div>
    </div>

    <div class="custom-block">
      <div class="custom-img">
        <img src="https://severplit.ru/thumb/2/pyK6LO3rn0yfaAhnxcVoXw/900r600/d/55112521_2.jpg"/>
      </div>
      <div class="custom-info">
        <div class="custom-info-title">
          <div class="align-self-center">
          Оптовые поставки
          </div>
        </div>
        <div class="">
          <div class="custom-title">
            Осуществляем оптовые поставки материалов и готовых изделий с гарантией качества и своевременной доставкой. Надежный партнёр для вашего бизнеса и крупных проектов.
          </div>
        </div>
        <button class="custom-button">
          Рассчитать стоимость изготовления →
        </button>
      </div>
    </div>

    <div class="custom-block">
      <div class="custom-img">
        <img src="https://severplit.ru/thumb/2/pyK6LO3rn0yfaAhnxcVoXw/900r600/d/55112521_2.jpg"/>
      </div>
      <div class="custom-info">
        <div class="custom-info-title">
          <div class="align-self-center">
          Розничные продажи
          </div>
        </div>
        <div class="">
          <div class="custom-title">
            В нашем ассортименте вы найдете качественные материалы и товары для вашего дома или мастерской. Доступные цены и персональный подход к каждому покупателю.
          </div>
<!--          <ul class="custom-list">-->
<!--            <li>-->
<!--              Распил (раскрой) плит по размерам заказчика-->
<!--            </li>-->
<!--            <li>-->
<!--              Кромлению  плитных материалов-->
<!--            </li>-->
<!--            <li>-->
<!--              Присадку (сверление) плит под мебельную фурнитуру-->
<!--            </li>-->
<!--          </ul>-->
        </div>
        <button class="custom-button">
          Рассчитать стоимость изготовления →
        </button>
      </div>
    </div>
  </div>
</template>

<script setup lang="ts">
import ScrollAnimation from "./ScrollAnimation.vue";


</script>

<style scoped>

h1 {
  margin-bottom: 20px;
}

.custom-title {
  font-size: 18px;
  height: 120px;
  text-align: center;
}

.w-100 {
  width: 100%!important;
}

.custom-block {
  width: 49.5%;
  padding: 10px;
  border: 0.1px solid gray;
  margin-top: 20px;
}

.custom-info-title {
  text-align: center;
  font-size: 22px;
  font-weight: bold;
  height: 60px;
  margin-bottom: 15px;
  display: flex;
  justify-content: center;
}

.custom-list {
  font-size: 16px;
}

.custom-img {
  display: flex;
  justify-content: center;
}

.custom-img img {
  max-width: 100%;
  margin-bottom: 40px;
  height: 100%;
}

.custom-button {
  margin-top: 20px;
  cursor: pointer;
  background-color: #606C38;
  padding: 15px 25px;
  font-size: 16px;
  color: #fff;
  border: none;
  transition: 0.3s;
}

.custom-button:hover {
  //transform: scale(1.05);
  background-color: #283618;
}

.custom-info {
  display: flex;
  flex-direction: column;
  justify-content: space-between;

}

</style>
