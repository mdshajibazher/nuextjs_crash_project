<template>

  <div class="container">
      <hero/>
      <large-card-display v-for="(cardinfo,index) in largeCardInfo" :key="index" :cardsSection="cardinfo"/>

      <small-card-display v-for="(cardinfo,index) in smallCardInfo" :key="'sc'+index" :cardsSection="cardinfo" />
  </div>
</template>

<script>
import {largeCardSections, smallCardSections} from '@/assets/data';
export default {

  data(){
    return {
      largeCardInfo: largeCardSections,
      smallCardInfo: smallCardSections,
    }
  }  
}
</script>

<style>


</style>
