<template>
  <div class="container">
    <div v-for="card in cards" :key="card">
      <Card :title="card.title" :tags="card.tags" :img="require(`@/assets/img/${card.img}`)" :description="card.description" :link="card.link" />
    </div>
  </div>
</template>

<script>
import Card from '@/components/Card'
import cards from '@/assets/card.json'

export default {
  components: {
    Card
  },
  data() {
    return {
      cards: cards
    }
  }
}
</script>

<style>
body {
  background-color: #e9ffe0; }
.container {
  padding-top: 70px;
  padding-right: 15px;
  padding-left: 15px;
  margin-right: auto;
  margin-left: auto;
  max-width: 1140px; }
.box {
  column-width: 400px; }
</style>