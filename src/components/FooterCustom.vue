<template>
  <div class="footer">
    <div class="footer-block">
      <div class="footer-item">
        <img src="@/assets/logo.svg" alt="logo" width="190px"/>
      </div>
      <div class="footer-item text-align-center">
         2010 - 2024
      </div>
    </div>
    <div class="footer-block">
      <div class="footer-item">
        2-я Квесисская ул., дом 23, Москва, Россия, 127220
      </div>
    </div>
    <div class="footer-block">
      <div class="footer-item">
        10:00 - 19:00
      </div>
    </div>
    <div class="footer-block">
      <div class="footer-item">
        <a class="telephone" href="tel:+79857046633">
          +7 (985) 704-66-33
        </a>
      </div>
    </div>
  </div>
</template>

<script setup lang="ts">

</script>

<style scoped>
.bg-white {
  background: #ffffff;
}

.footer {
  padding: 20px 0 40px 0;
  display: flex;
  justify-content: space-around;
  background: #606C38;
  color: #fff;
}

.footer-item {
  text-align: center;
}

.footer-block {
  width: 24%;
}

.telephone {
  font-weight: bold;
  font-size: 20px;
}

</style>
