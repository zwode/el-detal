<script setup lang="ts">
import NavBar from '@/components/NavBar.vue'
import SliderItem from '@/components/SliderItem.vue'
import MostPopularItems from '@/components/MostPopularItems.vue'
import WhyChoise from '@/components/WhyChoise.vue'
import HeaderCustom from '@/components/HeaderCustom.vue'
import FeedbackClient from '@/components/FeedbackClient.vue'
import AboutCompany from '@/components/AboutCompany.vue'
import FooterCustom from '@/components/FooterCustom.vue'
import selectAnimaitedItem from '@/components/selectAnimaitedItem.vue'
</script>

<template>
  <main>
    <HeaderCustom />
    <NavBar />
    <SliderItem />
    <AboutCompany />
    <MostPopularItems />
    <selectAnimaitedItem />
    <FeedbackClient />
    <div class="mt-2">

    </div>
    <FooterCustom />
  </main>
</template>
