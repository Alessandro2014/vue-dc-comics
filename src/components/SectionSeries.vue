<template>
  <div class="cards">
      <img :src="comic.thumb" :alt="comic.series">
      <figcaption>{{ comic.series }}</figcaption>   
    </div>
</template>

<script>
export default {
name:'SectionSeries',
props: ['comic']
}
</script>

<style scoped lang="scss">
.cards {
    height: auto;
    width: 200px;
    padding: 1rem;
    margin: 0 auto;
    
}
</style>