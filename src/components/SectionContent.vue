<template>
  <section>
      <div>
        <h3>Contenuto....</h3>  
      </div>
  </section>
</template>

<script>
export default {
    name:"SectionContent",
}
</script>

<style scoped lang="scss">
    section{
        position: relative;
        z-index: 2;
        height: 120px;
        background-color: black;
        div {
            max-width: 1300px;
            margin: 0 auto;
            line-height: 120px;
            
        }
    }
</style>