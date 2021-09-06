<template>
<footer id="footer-top">
    <section class="container">
        <div class="row">
            <nav>
                <h3>dc comics</h3>
                <ul>
                    <li><a href="">characters</a></li> 
                    <li><a href="">comics</a></li>
                    <li><a href="">movie</a></li>
                    <li><a href="">TV</a></li>
                    <li><a href="">games</a></li>
                    <li><a href="">videos</a></li>
                    <li><a href="">news</a></li>
                </ul>
            </nav>
            <figure>
                <img src="@/assets/img/dc-logo-bg.png" alt="">
            </figure>
      
        </div>
    </section>

    <section class="footer-bottom">

    </section>
</footer>
  
</template>

<script>
export default {
    name:"Footer"
}
</script>

<style scoped lang="scss">
    #footer-top {
        height: 500px;
        width: 100%;
        background-image: url("../assets/img/footer-bg.jpg");
     .container{
        max-width: 1300px;
        margin: 0 auto;
     .row {
        height: 450px;
        display: flex;
        align-items: center;
      }
     }
    }

     nav {
        h3 {
         color: white;
         text-transform: uppercase;
        ul {
            display: flex;
            flex-direction: column;
        li {
         list-style: none;
        a {
         text-decoration: none;
         padding: 5px;
         text-transform: capitalize;
         color: #464646;
         font-size: 0.7rem;
           }
          }
         }
        }
    }

    img {
           max-width: 100%; 
        }

</style>