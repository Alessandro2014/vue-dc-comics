<template>
<footer id="footer-top">
    <div class="container">
        <div class="row">
            <!-- LINK DI NAVIGAZIONE FOOTER -->
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
                <h3>shop</h3>
                <ul>
                    <li><a href="">shop DC</a></li> 
                    <li><a href="">shop DC collectibles</a></li>
                </ul>
            </nav>
            <nav>
                <h3>dc</h3>
                <ul>
                    <li><a href="">term of use</a></li> 
                    <li><a href="">privacy policy (new)</a></li>
                    <li><a href="">ad choices</a></li>
                    <li><a href="">advertising</a></li>
                    <li><a href="">jobs</a></li>
                    <li><a href="">subscription</a></li>
                    <li><a href="">talent workshops</a></li>
                    <li><a href="">CPSC certificates</a></li> 
                    <li><a href="">ratings</a></li>
                    <li><a href="">shop help</a></li>
                    <li><a href="">contact us</a></li>
                </ul>
            </nav>
            <nav>
                <h3>sites</h3>
                <ul>
                    <li><a href="">DC</a></li> 
                    <li><a href="">MAD magazine</a></li>
                    <li><a href="">DC kids</a></li>
                    <li><a href="">DC universe</a></li>
                    <li><a href="">DC power visa</a></li>
                </ul>
            </nav>
            <figure>
                <img src="../assets/img/dc-logo-bg.png" alt="">
            </figure>
        </div>
    </div>
</footer>
  
</template>

<script>
export default {
    name:"FooterTop"
}
</script>

<style scoped lang="scss">
@import "../assets/scss/_vars.scss";
#footer-top {
    height: 400px;
    width: 100%;
    background-image: url("../assets/img/footer-bg.jpg");
    position: relative;
    .container{
        max-width: 1300px;
        margin: 0 auto;
    }
}

nav {
    margin: 20px 25px 0 0;
    height: 400px;
h3 {
    margin: 15px 0;
    }
    ul {
    display: flex;
    flex-direction: column;
    li {
        list-style: none;
        margin-bottom: 5px;
        a {
        text-decoration: none;
        text-transform: capitalize;
        color: $gray-color;
    }
  } 
 }
}

figure {
    position: absolute; 
        top: -50px;
        right: 50px;
        z-index: 1;
    img {
        max-width: 90%;
    }
}
</style>