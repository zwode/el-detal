<template>
  <div>
    <div class="product-list">
      <div class="product">
        <div class="product-img mb-1">
          <img src="https://new.mato-plit.ru/ph_up/p649_1370_l.jpg">
        </div>
        <div class="product-title mb-1">
          ЛДСП Кроностар. Декор 1-я группа
        </div>
        <div class="product-sizes mb-1">
          <div>
            Размеры:
          </div>
          <div>
            <div class="product-size">
              2800х2070x16
            </div>
            <div class="product-size">
              2800х2070x16
            </div>
          </div>
        </div>
        <div class="price mb-1">
          <div class="mb-1">
            Цены:
          </div>
          <div class="d-flex justify-content-between mb-1">
            <div class="">
              За Кв.м:
            </div>
            <div class="font-weight-bold">
              578₽ - 625₽
            </div>
          </div>
          <div class="d-flex justify-content-between mb-1">
            <div class="">
              Лист:
            </div>
            <div class="font-weight-bold">
              3351₽ - 4625₽
            </div>
          </div>
          <div class="d-flex justify-content-between mb-1">
            <div class="">
              Паллета (33 листа):
            </div>
            <div class="font-weight-bold">
              110593₽ - 142625₽
            </div>
          </div>
          <div class="d-flex justify-content-between mb-1">
            <div class="">
              Фура (10 палет):
            </div>
            <div class="font-weight-bold">
              1105931₽ - 1305931₽
            </div>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script setup lang="ts">

</script>

<style scoped>

.product {
  width: 32%;
  border: 1px solid;
  padding: 10px;
}

.product-title {
  font-weight: bold;
}

.product-sizes {
  display: flex;
  justify-content: space-between;
}

.product-size {
  font-weight: bold;
}

.product-img img {
  width: 100%;
}

.d-flex {
  display: flex;
}

.mb-1 {
  margin-bottom: 1rem;
}

</style>
