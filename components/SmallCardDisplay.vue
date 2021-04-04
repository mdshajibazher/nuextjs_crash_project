<template>
  <div class="container">
      <div class="header">{{cardsSection.title}}</div>
      <div class="card-container">
          <SmallCard v-for="(card,index) in cardsSection.cards" :key="index" :card="card"/>
          
      </div>
  </div>
</template>

<script>

export default {
  props: ['cardsSection']
}
</script>

<style>

    .container {
        padding: 2rem 0
    }
    .header {
        font-weight: 700;
        font-size: 1.5rem;
        margin-bottom: 2rem;
    }
    .card-container {
        display: flex;
        justify-content: space-between;
        flex-wrap: wrap;
    }
</style>