<template>
  <div>
    <div class="d-flex justify-content-between mt-2">
      <h2>
        Популярные категории
      </h2>
      <div>
        Весь каталог
      </div>
    </div>
    <div class="d-flex justify-content-between">
      <div class="view-item">
        <img src="https://21vekst.ru/upload/iblock/e98/bbatb1q5246sbjmvh8itb89jmulnq4us.png" />
        <div class="view-item-text">
          Кромка ПВХ
        </div>
      </div>
      <div class="view-item">
        <img src="https://21vekst.ru/upload/iblock/9e7/ahoih605f36toduz0nkhauebtf1i01yd.png" />
        <div class="view-item-text">
          ДСП
        </div>
      </div>
      <div class="view-item">
        <img src="https://21vekst.ru/upload/iblock/876/vvplyfgpzidlaudm3lv72gg3ykeumuuv.png" />
        <div class="view-item-text">
          ЛДСП
        </div>
      </div>
      <div class="view-item">
        <img src="https://21vekst.ru/upload/iblock/3c4/qbc79747diz34d7z2ld71augk2gx0fqy.png" />
        <div class="view-item-text">
          ЛМДФ
        </div>
      </div>
    </div>
  </div>
</template>

<script setup lang="ts">

</script>

<style scoped>
.view-item {
  padding: 40px;
  background: #ffffff;
  box-shadow: 0px 1px 2px rgba(0, 0, 0, 0.1);
  margin-top: 10px;
  width: 24%;
  text-align: center;
  cursor: pointer;
  transition: 0.2s ease-in-out;
  border: 0.1px solid gray;
}

.view-item:hover {
  transform: scale(1.05);
  transition: all 0.2s ease-in-out;
  box-shadow: 0px 2px 10px rgba(0, 0, 0, 0.1);
}

.view-item-text {
  color: #000;
}

</style>
