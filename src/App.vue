<template>
  <div id="app">
    <Header/>
    <SectionJumbotron/>
    <SectionContent/>
    <Main/>
    <FooterTop/>
    <FooterBottom/>
  </div>
</template>

<script>
import Header from '@/components/Header.vue'
import SectionContent from '@/components/SectionContent.vue'
import Main from '@/components/Main.vue'
import FooterTop from '@/components/FooterTop.vue'
import FooterBottom from '@/components/FooterBottom.vue'
import SectionJumbotron from '@/components/SectionJumbotron.vue'


export default {
  name: 'App',
  components: {
    Header,
    SectionContent,
    Main,
    FooterTop,
    FooterBottom,
    SectionJumbotron,
  }
}
</script>

<style lang="scss">
@import "@/assets/scss/_vars.scss";
// UTILS
#app {
  font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
  -webkit-font-smoothing: antialiased;
}

* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;

}
// ISTRUZIONI GENERICHE
.container{
  max-width: 1300px;
  margin: 0 auto;
  .row {
    display: flex;
    align-items: center;
  }
}

li {
  list-style: none;
  a {
    text-decoration: none;
    color: $gray-color;
    text-transform: capitalize;
  }
}

h3 {
  color: white;
  text-transform: uppercase;
}
</style>
