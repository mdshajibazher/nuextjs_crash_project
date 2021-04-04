<template>
  <div class="container">
      <h4 class="header">{{cardsSection.title}}</h4>
      <p class="snippet">{{cardsSection.snippet}}</p>
      <div class="cards-container">
          <large-card v-for="(card,index) in cardsSection.cards" :key="index" :card="card"/>
      </div>
  </div>
</template>

<script>
export default {
    props:['cardsSection']
}
</script>

<style scoped>
.container {
    margin-top: 2rem;
    overflow: hidden;
}
    .header {
        font-weight: 700;
        font-size: 1.5rem;
    }
    .snippet {
        color: grey;
        margin-bottom: 1.5rem;
    }
    .cards-container {
        display: flex;
        justify-content: space-between;
    }
    .cards-container a{
        color: #000;
    }
</style>