<script setup lang="ts">
import NavBar from '@/components/NavBar.vue'
import SliderItem from '@/components/SliderItem.vue'
import MostPopularItems from '@/components/MostPopularItems.vue'
import WhyChoise from '@/components/WhyChoise.vue'
import CustomMaterial from '@/components/CustomMaterial.vue'
import HeaderCustom from '@/components/HeaderCustom.vue'
import FeedbackClient from '@/components/FeedbackClient.vue'
import AboutCompany from '@/components/AboutCompany.vue'
</script>

<template>
  <main>
    <HeaderCustom />
    <NavBar />
    <SliderItem />
    <CustomMaterial />
    <AboutCompany />
    <MostPopularItems />
    <WhyChoise />
    <FeedbackClient />
    <div class="mt-2">

    </div>
    <NavBar />
  </main>
</template>
