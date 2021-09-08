<template>
  <section class="series">
      <!-- CONTENITORE CARDS -->
        <section class="current-series container"> 
            <SectionSeries
            v-for="(comic, index) in dcComics" :key="index" :comic="comic"/>
        </section> 
        <h3 class="button">load moore</h3>
  </section>
</template>

<script>
import dcComics from "@/data/dcComics.js";
import SectionSeries from "@/components/SectionSeries.vue";

export default {
    name:"SectionContent",
    data() {
        return {
            // IMPORTO ARRAY DI OGGETTI FUMETTI CORRENTI
            dcComics,
        }
    },
    components: {
        SectionSeries,
    },
}
</script>

<style scoped lang="scss">
@import "../assets/scss/_vars.scss";

    .series{
        background-color: #1C1C1C;
        text-align: center;
        .current-series {
            padding-top: 3rem;
            display: flex;
            flex-wrap: wrap;
            color: white;
            padding-bottom: 10px;
        }   .button {
                margin: 30px 0;
                font-size: 0.9rem;
                padding: 10px;
                background-color: $blue-color;
                display: inline-block;
            }
    }

</style>