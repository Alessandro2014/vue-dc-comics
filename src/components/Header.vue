<template>
  <header class="container">
      <div class="row">
        <figure>
            <img src="@/assets/img/dc-logo.png" alt="logo">

        </figure>
        <nav>
            <ul>
                <li><a href="">characters</a></li>
                <li><a href="">comics</a></li>
                <li><a href="">movies</a></li>
                <li><a href="">tv</a></li>
                <li><a href="">games</a></li>
                <li><a href="">collectibles</a></li>
                <li><a href="">videos</a></li>
                <li><a href="">fans</a></li>
                <li><a href="">news</a></li>
                <li><a href="">shop</a></li>
            </ul>
        </nav>
    </div>
  </header>
</template>

<script>
export default {
    name: "Header",

}
</script>

<style lang="scss">
    
    .container{
        max-width: 1300px;
        margin: 0 auto;
        .row {
            height: 110px;
            display: flex;
            justify-content: space-between;
            align-items: center;
     
        img {
            max-width: 70px;
            height: auto;
        }
        }
    }

    nav {
         ul {
         display: flex;
            justify-content: space-between;
            align-items: center;
        li {
         list-style: none;
         font-weight: bold;
        a {
         text-decoration: none;
         padding: 10px;
         text-transform: uppercase;
         color: #464646;
         &:hover {
            color: #0282F9;
            }
          }
         }
        }
    }
</style>