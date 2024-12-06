<template>
  <div ref="element" class="box" :class="{ visible: isVisible }">
    <slot />
  </div>
</template>

<script lang="ts" setup>

import { ref, onMounted, onUnmounted } from "vue";

const element = ref(null);
const isVisible = ref(false);

const handleScroll = () => {
  if (!element.value) return;

  const rect = element.value.getBoundingClientRect();
  const windowHeight = window.innerHeight;

  // Если элемент виден хотя бы на 50%
  if (rect.top <= windowHeight * 0.75 && rect.bottom >= windowHeight * 0.25) {
    isVisible.value = true;
  }
};

onMounted(() => {
  window.addEventListener("scroll", handleScroll);
  handleScroll();
});

onUnmounted(() => {
  window.removeEventListener("scroll", handleScroll);
});
</script>

<style scoped>
.box {
  opacity: 0;
  transform: translateX(1000px);
  transition: all 2s ease-in-out;
}

.box.visible {
  opacity: 1;
  transform: translateY(0);
}
</style>
