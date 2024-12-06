<template>
  <div class="d-flex mt-2 custom-block">
    <div class="custom-img">
      <img src="https://severplit.ru/thumb/2/pyK6LO3rn0yfaAhnxcVoXw/900r600/d/55112521_2.jpg"/>
    </div>
    <div class="custom-info">
      <h1>
        Распил и кромление
      </h1>
      <div class="">
        <div class="custom-title"> Предлагаем нашим клиентам дополнительные услуги: </div><br>
        <ul class="custom-list">
          <li>
            Распил (раскрой) плит по размерам заказчика
          </li>
          <li>
            Кромлению  плитных материалов
          </li>
          <li>
            Присадку (сверление) плит под мебельную фурнитуру
          </li>
        </ul>
      </div>
      <button class="custom-button">
        Рассчитать стоимость изготовления →
      </button>
    </div>
  </div>
</template>

<script setup lang="ts">

</script>

<style scoped>

h1 {
  margin-bottom: 20px;
}

.custom-title {
  font-size: 18px;
}

.custom-list {
  font-size: 16px;
}

img {
  width: 600px
}

.custom-img {
  margin-right: 20px;
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
  background-color: #6f4518;
}

.custom-info {
  display: flex;
  flex-direction: column;
  justify-content: space-between;

}

</style>
