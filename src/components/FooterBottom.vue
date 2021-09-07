<template>
  <footer id="footer-bottom">
      <div class="container">
        <div class="row">
            <div class="link-sign">
                <h3>SIGN-UP NOW!</h3>
            </div>
            <div class="social">
                <h3>follow us</h3>
                <img src="@/assets/img/footer-facebook.png" alt="facebook">
                <img src="@/assets/img/footer-twitter.png" alt="twitter">
                <img src="@/assets/img/footer-youtube.png" alt="youtube">
                <img src="@/assets/img/footer-pinterest.png" alt="pinterest">
                <img src="@/assets/img/footer-periscope.png" alt="periscope">
            </div>
        </div>
      </div>
  </footer>
</template>

<script>
export default {
    name:"FooterBottom"
}
</script>

<style scoped lang="scss">
    #footer-bottom {
        position: relative;
        z-index: 2;
        height: 120px;
        background-color: #303030;
    }

.container .row {
    justify-content: space-between;
    height: 120px;
    align-content: center;
}



.link-sign {
    border: 2px;
    padding: 10px;
    border-color: #0282F9;
}

.social {
    width: 400px;
    display: flex;
    justify-content: space-between;
    align-items: center;
}

.social h3 {
    color: #0282F9;
}
</style>