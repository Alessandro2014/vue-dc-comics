<template>
    <div>
        <div class="cards">
            <img :src="comic.thumb" :alt="comic.series">
            <figcaption>{{ comic.series }}</figcaption>   
        </div>
    </div>
  
</template>

<script>
export default {
name:'SectionSeries',
props: ['comic']
}
</script>

<style scoped lang="scss">
@import "../assets/scss/_vars.scss";
.cards {
    height: auto;
    width: 200px;
    padding: 1rem;
    margin: 0 auto;
    text-align: initial;
    img {
        width: 100%;
    }
}

</style>