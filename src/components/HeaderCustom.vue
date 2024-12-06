<template>
  <div class="d-flex mt-2 justify-content-between align-items-center">
    <div class="header-logo">
      <img src="@/assets/logo.svg" alt="logo" width="190px"/>
    </div>
    <div class="header-search align-self-center d-flex">
     <input placeholder="Поиск" />
      <div>
        <img src="@/components/icons/icons8-search.svg" alt="search" width="25px" height="25px" />
      </div>
    </div>
    <div class="align-self-center header-phone">
      <a href="tel:77072001411">
        +7 (707) 777 20 11
      </a>
    </div>
    <div class="header-cart align-self-center">
      <img src="@/assets/cart.png" alt="cart" width="30px" height="30px" />
    </div>
  </div>
</template>

<script setup lang="ts">

</script>

<style scoped>
.header-logo {
  width: 190px;
  height: 40px;
  position: relative;
}

a {
  color: #2c3e50!important;
}

.header-phone {
  font-weight: bold;
  font-size: 20px;
  padding-top: 5px;
  margin-left: 15px;
}

.header-logo img {
  position: absolute;
  top: -41px;
  left: -35px;
  width: 150px;
}

.header-search {
  border-radius: 0;
  height: 35px;
  width: 40%;
  border: 0.5px solid #7f878f;
  padding: 5px 10px;
}

.header-search input {
  border: none;
  width: 100%;
  background: none;
}

.header-cart {
  border: 0.5px solid transparent;
  padding: 5px;
}

.header-cart:hover {
  border: 0.5px solid #7f878f;
}

</style>
