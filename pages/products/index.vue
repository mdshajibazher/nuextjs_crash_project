<template>
    <div class="container">
        <large-card-display v-for="(cardinfo,index) in largeCardInfo.slice(0,1)" :key="index" :cardsSection="cardinfo"/>
            <small-card-display v-for="(cardinfo,index) in smallCardInfo.slice(0,1)" :key="'sc'+index" :cardsSection="cardinfo" />
    </div>

</template>

<script>
import {largeCardSections, smallCardSections} from '@/assets/data'
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