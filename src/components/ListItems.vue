<template>
  <div class="list-group">
    <div class="d-flex">
      <div :class="{ 'active': isActive }" @click="changeView()">
        Плитка
      </div>
      <div :class="{ 'active': !isActive }" @click="changeView()">
        Таблица
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

</style>
