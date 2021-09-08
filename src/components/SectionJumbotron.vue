<template>
<!-- JUMBOTRON SOTTO HEADER CON PLACEHOLDER -->
    <div class="jumbotron">
        <h3 class="placeholder">current series</h3>
    </div>
  
</template>

<script>
export default {
name:'SectionJumbotron',
}
</script>

<style scoped lang="scss">
@import "../assets/scss/_vars.scss";
.jumbotron{
    background-image: url('../assets/img/jumbotron.jpg');
    height: 400px;
}

.placeholder {
    padding: 10px;
    position: absolute;
    left: 10%;
    top: 500px;
    padding: 10px;
    background-color: $blue-color;
    display: inline-block;
}

</style>