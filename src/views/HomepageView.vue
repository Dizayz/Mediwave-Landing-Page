<script setup lang="ts">
import HeaderSection from "../components/Homepage/HeaderSection.vue"
import ContentSection from "../components/Homepage/ContentSection.vue";
import SwiperSection from '../components/Homepage/SwiperSection.vue'
import FonctionnaliteSection from "@/components/Homepage/FonctionnaliteSection.vue";
import MobileAppSection from '../components/Homepage/MobileAppSection.vue'
import LastSection from '../components/Homepage/LastSection.vue'
import FooterSection from "../components/Homepage/FooterSection.vue"
</script>

<template>
  <main>
    <HeaderSection></HeaderSection>
    <ContentSection></ContentSection>
    <SwiperSection></SwiperSection>
    <FonctionnaliteSection></FonctionnaliteSection>
    <MobileAppSection></MobileAppSection>
    <LastSection></LastSection>
    <FooterSection></FooterSection>
  </main>
</template>
<style scoped></style>

