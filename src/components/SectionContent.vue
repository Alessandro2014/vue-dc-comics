<template>
  <section class="series">
        <section class="current-series container">
            <SectionSeries
            v-for="(comic, index) in dcComics" :key="index" :comic="comic"/>
        </section>  
  </section>
</template>

<script>
import dcComics from "@/data/dcComics.js";
import SectionSeries from "@/components/SectionSeries.vue";

export default {
    name:"SectionContent",
    data() {
        return {
            dcComics,
        }
    },
    components: {
        SectionSeries,
    },
}
</script>

<style scoped lang="scss">
    .series{
        background-color: #1C1C1C;
        .current-series {
            padding: 3rem 0;
            display: flex;
            flex-wrap: wrap;
            color: white;
        }
    }
</style>