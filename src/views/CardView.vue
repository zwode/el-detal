<template>
  <div class="list-group">
    <div class="d-flex justify-content-between">
      <div>
        Вид:
      </div>
      <div class="d-flex">
        <div class="select-view" :class="{ 'active': isActive }" @click="changeView()">
          <img src="@/assets/plita.png" alt="plate">
        </div>
        <div class="select-view" :class="{ 'active': !isActive }" @click="changeView()">
          <img src="@/assets/table.png" alt="table">
        </div>
      </div>
    </div>
    <div v-if="viewStatus">
      <CardItem />
    </div>
    <div v-else>
      <TableItem />
    </div>
  </div>
</template>

<script setup lang="ts">
import CardItem from '@/components/CardItem.vue'
import TableItem from '@/components/TableItem.vue'
import { ref } from 'vue'
import type { Ref } from 'vue'

const viewStatus: Ref <boolean> = ref(true)
const isActive: Ref<boolean> = ref(true)

function changeView(): void {
  viewStatus.value = !viewStatus.value;
  isActive.value = !isActive.value
}
</script>

<style scoped>

.select-view {
  transition: all 0.2s ease-in-out;
  padding: 10px;
  margin-right: 10px;
  border: 1px solid transparent;
}

.select-view:hover {
  transform: scale(1.05);
  border: 1px solid #606C38;
}

.select-view.active {
  border: 1px solid #606C38;
}

.select-view img {
  width: 25px;
  height: 25px;
}

</style>
