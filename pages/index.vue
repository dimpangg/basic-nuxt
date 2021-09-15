<template>
  <div>
    <Nav />
    <b-container fluid>
      <hero />
      <LargeCardDisplay
        v-for="cardInfo in largeCardInfo"
        :key="cardInfo.id"
        :cardSection="cardInfo"
      />
      <SmallCardDisplay
        v-for="cardInfo in smallCardSections"
        :key="cardInfo.id"
        :cardSection="cardInfo"
      />
    </b-container>
  </div>
</template>

<script>
import { largeCardSections, smallCardSections } from "@/assets/data.js";

export default {
  data() {
    return {
      largeCardInfo: largeCardSections,
      smallCardSections,
    };
  },
};
</script>
