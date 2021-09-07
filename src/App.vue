<template>
  <div id="app">
    <Header/>
    <SectionContent/>
    <Main/>
    <FooterTop/>
    <FooterBottom/>
  </div>
</template>

<script>
import Header from './components/Header.vue'
import SectionContent from './components/SectionContent.vue'
import Main from './components/Main.vue'
import FooterTop from './components/FooterTop.vue'
import FooterBottom from './components/FooterBottom.vue'

export default {
  name: 'App',
  components: {
    Header,
    SectionContent,
    Main,
    FooterTop,
    FooterBottom,
  }
}
</script>

<style lang="scss">
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
}

* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}

.container{
  max-width: 1300px;
  margin: 0 auto;
}

.row {
  display: flex;
  align-items: center;
}

li {
  list-style: none;
}

a {
  text-decoration: none;
  color: #9c9c9c;
  font-size: 0.8rem;
  text-transform: capitalize;
}

h3 {
  color: white;
  text-transform: uppercase;

}
</style>
